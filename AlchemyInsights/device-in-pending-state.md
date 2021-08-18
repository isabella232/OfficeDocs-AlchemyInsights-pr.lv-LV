---
title: Ierīce ir gaidošā stāvoklī
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: 7d8a55f8c9a9fc30c653152c2f1b185874cea3ee
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330379"
---
# <a name="device-in-pending-state"></a>Ierīce ir gaidošā stāvoklī

**Priekšnosacījumi:**

1. Ja iestatāt ierīču reģistrācijas pirmo reizi, pārliecinieties, vai esat pārskatījis Ievads par ierīču pārvaldību programmā [Azure Active Directory (Azure AD),](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) kas palīdzēs iegūt ierīces Azure AD kontrolē.
2. Ja reģistrējat ierīces Azure AD tieši un reģistrējat tās Intune, jums vispirms ir jākonfigurē [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) un vispirms jāveic licencēšana. [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support)
3. Pārliecinieties, vai esat pilnvarots veikt darbības Azure AD un lokālajā AD. Ierīču reģistrāciju iestatījumus var pārvaldīt tikai Azure Active Directory globālais administrators. Turklāt, ja iestatāt automātiskas reģistrācijas lokālajā Active Directory, jums būs jābūt Active Directory un AD FS administratoram (ja piemērojams).

Hibrīda Azure AD pievienošanās reģistrācijas procesam nepieciešamas ierīces uzņēmuma tīklā. Tas darbojas arī, izmantojot VPN, bet tas arī tiek darīts. Esam informējuši klientus, ka ir nepieciešama palīdzība ar hibrīdā Azure AD pievienošanās reģistrācijas procesa problēmu novēršanu attālos darba apstākļos.

**Mākoņa autentifikācijas vide (izmantojot Azure AD paroles jaukšanas sinhronizāciju vai tranzīta autentifikāciju)**

Šī reģistrācijas plūsma tiek dēvēta arī par "Sinhronizācijas savienojums".

Lūk, kas notiek reģistrācijas procesa laikā:

1. Windows 10 atklāj pakalpojuma savienojuma punkta (Service Connection Point — SCP) ierakstu, kad lietotājs piesakās ierīcē.

    1. Ierīce vispirms mēģina izgūt nomnieka informāciju no klienta puses SCP reģistrā [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Papildinformāciju skatiet [dokumentā](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Ja tas neizdodas, ierīce sazinās ar lokālo Active Directory, lai iegūtu nomnieka informāciju no SCP. Lai pārbaudītu SCP, skatiet šo [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).

    **Piezīme.** Iesakām iespējot SCP Active Directory, tikai izmantojot klienta puses SCP sākotnējai validācijai.

2. Windows 10 sazināties ar Azure AD sistēmas kontekstā, lai autentificētos azure AD.

    Varat pārbaudīt, vai ierīce var piekļūt Microsoft resursiem sistēmas kontā, izmantojot ierīces [reģistrācijas testa skriptu](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. Windows 10 ģenerē pašparakstītu sertifikātu un saglabā to zem datora objekta lokālajā Active Directory. Domēna kontrollerim ir jābūt redzamam līnijai.

4. Ierīces objekts, kuram ir sertifikāts, tiek sinhronizēts ar Azure AD, izmantojot Azure AD Savienošana. Sinhronizācijas cikls pēc noklusējuma ir ik pēc 30 minūtēm, bet tas ir atkarīgs no Azure AD Savienošana. Papildinformāciju skatiet šajā [dokumentā.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. Šajā posmā temata ierīcei vajadzētu būt redzamai stāvoklī **"Gaida",** kas atrodas Azure Portal sadaļas Ierīces asmensmis.

6. Nākamajā lietotāja pieteikšanās reizē Windows 10 pabeigta reģistrācija.

    **Piezīme.** Ja izmantojat VPN un logoff/login, domēna savienojamība tiek pārtraukta, varat aktivizēt reģistrāciju manuāli. Lai to paveiktu:
    
    Problēma lokāli `dsregcmd /join` administratora uzvednē vai attāli, izmantojot PSExec jūsu datoram.\
    Piemērs. `PsExec -s \\win10client01 cmd, dsregcmd /join`

Bieži sastopamās problēmas saistībā ar Azure Active Directory reģistrāciju skatiet rakstā Bieži [uzdotie jautājumi par ierīcēm.](https://docs.microsoft.com/azure/active-directory/devices/faq)
