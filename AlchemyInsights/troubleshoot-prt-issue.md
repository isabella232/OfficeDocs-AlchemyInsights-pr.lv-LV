---
title: PRT problēmas novēršana
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: fd285d1158d7b358e4c698cf6014422cc2fb536e1fbdf98630bebda359f9c553
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972723"
---
# <a name="troubleshoot-prt-issue"></a>PRT problēmas novēršana

Lai jebkura ierīce pabeigtu autentificēšanu, tai jābūt pilnībā reģistrētai un labā stāvoklī, kā arī tai ir jābūt iespējai iegūt primāro atsvaidzināšanas pilnvaru (Primary Refresh Token — PRT).

Hibrīda Azure AD pievienošanās reģistrācijas procesam nepieciešamas ierīces uzņēmuma tīklā. Tas darbojas arī, izmantojot VPN, bet tas arī tiek darīts. Esam uzklausījuši klientus, kuriem nepieciešama palīdzība ar hibrīdā Azure AD pievienošanās reģistrācijas procesa problēmu novēršanu attālā darba apstākļos. Reģistrācijas procesa laikā tiek sadalījumu tam, kas notiek.

**Mākoņa autentifikācijas vide (izmantojot Azure AD paroles jaukšanas sinhronizāciju vai tranzīta autentifikāciju)**

Šī reģistrācijas plūsma tiek dēvēta arī par "Sinhronizācijas savienojums".

1. Windows 10 atklāj SCP ierakstu, kad lietotājs piesakās ierīcē.
    1. Ierīce vispirms mēģina izgūt nomnieka informāciju no klienta puses SCP reģistrā [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Papildinformāciju skatiet šajā [dokumentā.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)
    2. Ja tas neizdodas, ierīce sazinās ar lokālo Active Directory (AD), lai iegūtu nomnieka informāciju no pakalpojumu savienojuma punkta (Service Connection Point — SCP). Lai pārbaudītu SCP, skatiet šo [dokumentu.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point) 

> [!NOTE]
> Iesakām iespējot SCP AD un tikai izmantot klienta puses SCP sākotnējai validācijai.

2. Windows 10 mēģina sazināties ar Azure AD sistēmas kontekstā, lai autentificētos azure AD. Varat pārbaudīt, vai ierīce var piekļūt Microsoft resursiem sistēmas kontā, izmantojot ierīces reģistrācijas testa skriptu.

3. Windows 10 ģenerē pašparakstītu sertifikātu un saglabā to datora objektā lokālajā AD. Domēna kontrollerim ir jābūt redzamam līnijai.

4. Ierīces objekts, kuram ir sertifikāts, tiek sinhronizēts ar Azure AD, izmantojot Azure AD Savienošana. Sinhronizācijas cikls pēc noklusējuma ir ik pēc 30 minūtēm, bet tas ir atkarīgs no Azure AD Savienošana. Papildinformāciju skatiet šajā [dokumentā.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. Šajā posmā tēmas ierīcei vajadzētu būt redzamai stāvoklī "Gaida" azure portāla sadaļas Ierīces asmensmis.

6. Nākamajā lietotāja pieteikšanās reizē Windows 10 pabeigta reģistrācija. 

> [!NOTE]
> Ja izmantojat VPN un logoff pieteikšanās process pārtrauc domēna savienojamību, varat aktivizēt reģistrāciju manuāli:
 1. Izsniedziet dsregcmd /join lokāli administratora uzvednē vai attāli, izmantojot PSExec savā datorā. Piemēram, PsExec -s \\ win10client01 cmd, dsregcmd /join

 2. Papildinformāciju par hibrīdās pievienošanās problēmām skatiet rakstā [Ierīču problēmu novēršana.](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)
