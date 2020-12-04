---
title: Ar PRT problēmu saistītu problēmu novēršana
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
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573719"
---
# <a name="troubleshoot-prt-issue"></a>Ar PRT problēmu saistītu problēmu novēršana

Lai jebkura ierīce pabeigtu autentificēšanu, tai ir jābūt pilnībā reģistrētai un labā stāvoklī, kā arī var iegūt primāru atsvaidzināšanas marķieri (PRT).

Hibrīdā Azure AD pievienoties reģistrācijas procesam ir nepieciešamas ierīces, lai tās būtu korporatīvajā tīklā. Tā darbojas arī uz VPN, bet tam ir daži brīdinājumi. Mēs esam dzirdējuši, ka klientiem ir jāsniedz palīdzība saistībā ar Hibrīdā Azure AD Join reģistrācijas procesu attālā darba apstākļos. Tālāk ir sniegts to darbību sadalījums, kas notiek ar kapuci reģistrācijas procesa laikā.

**Mākoņa autentifikācijas vide (izmantojot Azure AD Password hash Sync vai tranzīta autentifikāciju)**

Šo reģistrācijas plūsmu dēvē arī par sinhronizācijas savienojumu.

1. Windows 10 atklāj SCP ierakstu, kad lietotājs pierakstās ierīcē.
    1. Ierīce vispirms mēģina izgūt nomnieka informāciju no klienta puses SCP reģistrā [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Lai iegūtu papildinformāciju, skatiet šo [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    2. Ja tas nelīdz, ierīce komunicē ar lokālo Active Directory (AD), lai iegūtu nomnieka informāciju no pakalpojumu savienojuma punkta (SCP). Lai verificētu SCP, lūdzu, skatiet šo [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point). 

> [!NOTE]
> Iesakām iespējot SCP reklāmas un tikai tad, izmantojot klienta puses SCP sākotnējai validācijai.

2. Windows 10 mēģina sazināties ar Azure AD, izmantojot sistēmas kontekstu, lai autentificētu sevi pret Azure AD. Varat pārbaudīt, vai ierīce var piekļūt Microsoft resursiem sistēmas kontā, izmantojot testa ierīces reģistrācijas savienojamības skriptu.

3. Windows 10 izveido pašparakstītu sertifikātu un saglabā to zem datora objekta lokālajā REKLĀMā. Lai to izdarītu, ir nepieciešams domēna kontrolleris.

4. Ierīces objekts, kura sertifikāts tiek sinhronizēts ar Azure AD, izmantojot Azure AD Connect. Sinhronizācijas cikls ik pēc noklusējuma ir 30 minūtes, tomēr tas ir atkarīgs no Azure AD Connect konfigurēšanas. Lai iegūtu papildinformāciju, lūdzu, skatiet šo [dokumentu](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. Šajā posmā varat skatīt tēmas ierīci sadaļā "gaida", sadaļā ierīces disks Azure Portal.

6. Nākamajā lietotāja pierakstīšanās operētājsistēmā Windows 10 reģistrācija tiks pabeigta. 

> [!NOTE]
> Ja esat pieslēdzies VPN, bet atteikšanās process pārtrauc domēna savienojamību, varat manuāli aktivizēt reģistrāciju:
 1. Dsregcmd/Join lokāli uz administratora uzaicinājuma vai attālināti, izmantojot PSExec savā datorā. Piemēram, PsExec-s \\ win10client01 cmd, dsregcmd/Join

 2. Detalizētu informāciju par Hibrīdajām problēmām skatiet rakstā [ierīču problēmu novēršana](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).
