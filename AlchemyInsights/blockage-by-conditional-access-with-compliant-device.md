---
title: Es saņemu bloķēšanu ar ierobežotu piekļuvi, kas atbilst ierīcei
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 240bd25f4d62505202c8cd7ceabe4c1cd3d5c0b5
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035997"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Es saņemu bloķēšanu ar ierobežotu piekļuvi, kas atbilst ierīcei

**Ļoti Ieteicamie rīki**

- [Ierīču reģistrācijas problēmu risinātāja rīks](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) — visaptverošs rīks, kas palīdz novērst izplatītākās ierīču reģistrācijas problēmas.
- [Ierīces reģistrācijas savienojamības skripta pārbaude](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) — rīks, kas tiek izmantots, lai nodrošinātu, ka ierīce var piekļūt ierīces reģistrācijas galapunktiem, kas atrodas sistēmas kontā.
- [AZURE ad Device cleanup skripts](https://github.com/mzmaili/AzureADDeviceCleanup) — rīks, kas tiek izmantots, lai meklētu un pārvaldītu novecojušas ierīces savā vidē.

Tālāk ir norādīti daži vispārīgi iemesli, kāpēc Nosacījumformatēšana var neizdoties atbilstošai ierīcei vai kāpēc lietotāji var saņemt ziņojumu pierakstīšanās pieprasījuma laikā **no šejienes** .

1. **Ierīce nav pieprasītā ierīces stāvoklī ar MDM**:

Pārbaudiet, vai ierīce ir reģistrēta pie apstiprināta MDM pakalpojumu sniedzēja, piemēram, Intune un *atzīmēts kā atbilstošs*. Papildinformāciju par Intune skatiet šajā [dokumentā](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment). Lai uzlabotu izpratni par ierīces saderību un Intune, skatiet rakstu [atbilstības politikas izmantošana, lai iestatītu kārtulas ierīcēm, kuras pārvaldāt ar Intune](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started). Ja rodas problēmas, pierakstot ierīci ar Intune, atrodiet informāciju par problēmu novēršanu [rakstā Ierīču reģistrācijas problēmu novēršana programmā Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune). Lai iegūtu papildu Intune atbalstu, izveidojiet atbalsta pieprasījumu. Lai to izdarītu, apmeklējiet [Intune palīdzības un atbalsta lapu](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).

2. **Ierīce nav savienota ar organizāciju tīklu**:

Lai piekļūtu organizācijas resursiem, ierīcei ir jābūt savienotai ar organizācijas tīklu, izmantojot tiešo savienojumu vai virtuālo privāto tīklu (VPN), kā arī savienoti ar lokālo vai Azure Active Directory. Lai pievienotos darba ierīcei organizācijas tīklā, skatiet rakstu [pievienošanās darba ierīcei savas organizācijas tīklā](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network). Lai reģistrētu personisko/BYOD ierīci, skatiet rakstu [personiskās ierīces reģistrēšana savas organizācijas tīklā](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network).

- Lai pārbaudītu, vai ierīce ir savienota ar tīklu, varat veikt tālāk norādītās darbības, lai reģistrētu ierīces [šeit](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) vai darba [ierīcēs.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined) Lai aptvertu problēmu ar organizācijas tīkla savienojamību, izpildiet tālāk sniegtos norādījumus.

    1. Pierakstieties sistēmā Windows, izmantojot savu darba vai mācību iestādes kontu, piemēram, alain@contoso.com.
    2. Izveidojiet savienojumu ar savas organizācijas tīklu, izmantojot VPN vai DirectAccess.
    3. Kad ir izveidots savienojums, nospiediet **Windows logotipa taustiņu + L** , lai bloķētu ierīci.
    4. Atbloķējiet ierīci, izmantojot savu darba vai mācību kontu, un pēc tam vēlreiz mēģiniet piekļūt problemātiskajai programmai vai pakalpojumam.

Ja tiek rādīts kļūdas ziņojums **no** šī paziņojuma par šo problēmu, iespējams, ir pieejama arī citur.

3. **Operētājsistēma netiek atbalstīta**:

Pārliecinieties, vai izmantojat operētājsistēmas atbalstīto versiju, tostarp:

- **Windows klients**: Windows 7 vai jaunāka versija

- **Windows Server**: windows Server 2008 R2 vai jaunāka versija

- **MacOS**: MacOS X vai jaunāka versija

- **Android un iOS**: jaunākā Android un iOS mobilo operētājsistēmu versija

4. **Tīmekļa pārlūkprogramma netiek atbalstīta**:

Lūdzu, atrodiet atbalstītās pārlūkprogrammas zemāk. Lai iegūtu Chrome atbalstu ar Windows 1703 vai jaunākām versijām, nepieciešams Windows 10 kontu paplašinājums. Ja jums ir jāpierakstās, lai uzzinātu, vai jums ir nepieciešams pierakstīties. Papildinformāciju skatiet [šeit](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

- **Windows 10**: Microsoft Edge, Internet Explorer, Chrome
- **Windows 8/8,1**: Internet Explorer, Chrome
- **Windows 7**: Internet Explorer, Chrome
- **iOS**: Microsoft Edge, Intune Managed Browser, Safari
- **Android**: **Microsoft Edge**: Intune Managed Browser, Chrome
- **Windows Phone**: Microsoft Edge, Internet Explorer
- **Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016**: Internet Explorer
- **Windows Server 2012 R2**: Internet Explorer
- **Windows Server 2008 R2**: Internet Explorer
- **macOS**: Chrome, Safari

Papildinformāciju skatiet [šeit](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation): šeit **nevar saņemt** ziņojumus un problēmu novēršanas darbības.
