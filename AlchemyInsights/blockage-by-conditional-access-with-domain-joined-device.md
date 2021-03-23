---
title: Es saņemu bloķētu piekļuvi, izmantojot domēna pieslēgto ierīci
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/20/2021
ms.locfileid: "51036701"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a>Es saņemu bloķētu piekļuvi, izmantojot domēna pieslēgto ierīci

**Ļoti Ieteicamie rīki**

[Ierīču reģistrācijas problēmu risinātāja rīks](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) — rīks, kas palīdz novērst izplatītākās ierīču reģistrācijas problēmas.

[Testa ierīces reģistrācijas savienojamības skripts](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) — skripts, kas nodrošina, ka ierīce var piekļūt ierīces reģistrācijas galapunktiem sistēmas kontā.

[AZURE ad Device cleanup skripts](https://github.com/mzmaili/AzureADDeviceCleanup) — skripts, kas sniedz iespēju meklēt un pārvaldīt novecojušas ierīces savā vidē.

Tālāk ir norādīti daži raksturīgākie iemesli, kāpēc Nosacījumformatēšana var bojāt ierīci, kas ir savienota ar domēnu (hibrīdais Azure AD).

1. **Ierīcē nav AZURE ad PRT** , ir jāpārliecinās, vai ierīcei ir Azure AD primārās atsvaidzināšanas pilnvara (PRT). Papildinformāciju par PRT skatiet šajā [dokumentā](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

Lai pārbaudītu, vai jums ir Azure AD PRT, varat izpildīt `dsregcmd/status` ierīces komandu un pārbaudīt, vai "AzureAdPrt" ir vienāds ar "Jā".

Ja "AzureAdPrt" ir "nē", pārbaudiet tālāk norādīto informāciju.

- **Neatkarīgi no tā, vai jums ir ārēja vide ar AD FS, un tas nav sasniedzams no lietotāju mājas tīkliem**: šajā gadījumā pārliecinieties, vai jūsu "usernamemixed" galapunkti ir pieejami no ārtīkla. Ja jūsu AD FS ir fonā, pārliecinieties, vai lietotāji izveido savienojumu ar VPN un atkārtoti pieteicies ierīcē. Lai iegūtu papildinformāciju, skatiet šo [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).

- Neatkarīgi no tā, **vai ierīces TPM ir kļūdains, tāpēc nevar autentificēt ierīci**: Check "TPM. msc", lai noskaidrotu, vai TPM statuss ir gatavs. Ja nav, palaidiet `dsregcmd/leave` un ļaujiet ierīcei atkārtoti pievienoties pakalpojumam AZURE ad. Pēc tam mēģiniet vēlreiz. Lai iegūtu papildinformāciju, skatiet šo [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).

- **Jūs izmantojat trešo personu identitātes pakalpojumu sniedzēju, kas neatbalsta WS-Trust protokolu**. Kā aprakstīts mūsu dokumentos, hibrīdās Azure AD-Savienotās ierīces nevar darboties šajā gadījumā. Lai saņemtu atbalstu, lūdzu, sazinieties ar savu identitātes nodrošinātāju.

2. **Lietotāji izmanto Chrome pārlūkprogrammu bez Windows 10 kontiem** vai **Office Extension Chrome automātiski neizmanto PRT ar AAD-savienotām vai hibrīdām ierīcēm**: tas rada jebkādas ierīces, kuru pamatā ir ierobežotas piekļuves politikas, tiek parādīts kļūdas ziņojums "nereģistrēta ierīce". Lai pareizi izmantotu Chrome pārlūkprogrammu, ir jāinstalē Windows 10 konti vai Office paplašinājums lietotāju Chrome pārlūkprogrammā, izmantojot SCCM vai Intune. Lai iegūtu papildinformāciju, skatiet šo [dokumentu](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

Ja nav iespējams veikt pagarinājumu attālināti, informējiet lietotājus par to, ka manuāli jāinstalē kāds no iepriekš norādītajiem paplašinājumiem, lai piekļūtu lietojumprogrammas, kuru pamatā ir ierīces piekļuve. Lai iegūtu papildinformāciju, skatiet šo [dokumentu](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).

3. **Ierīce bija pareizi pievienota Hibrīdā AZURE AD, bet tā ir nejauši izdzēsta vai atspējota, vai nu sakarā ar sinhronizācijas izmaiņām AZURE ad Connect vai Azure portālā**: ja tā notiek, ierīces objekts vairs netiek atpazīts kā pilnībā pievienota ierīce, lai gan "AzureAdJoined", gan "PRT" statuss ierīcē tiek rādīts kā derīgs.

Lai novērstu šo problēmu, palaidiet `dsregcmd/leave` ietekmētās ierīces un atdodiet tās AZURE ad. Lai iegūtu papildinformāciju, skatiet šo [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).

> [!NOTE]
> Ja jūsu ierīces darbojas operētājsistēmā Windows 10, 1809 atjauninājums ar VPN/Cloud starpniekserveri un redzamas problēmas ar "AzureAdPrt" vai kādu programmu ar SSO problēmu (Outlook neveido savienojumu ar pastkasti pat tad, ja ir bijusi PRT), pārliecinieties, vai jums ir šis plāksteris [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) vai aprīļa kumulatīvās atjaunināšanas [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) , lai novērstu PRT nepilnības šajos datoros.

















