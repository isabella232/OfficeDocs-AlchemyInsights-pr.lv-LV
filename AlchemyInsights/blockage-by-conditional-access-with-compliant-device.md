---
title: Nosacījum access ar atbilstošu ierīci mani bloķē
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
ms.openlocfilehash: 709749b1a62f2d9cdabfb3fe4b7538c22101d7109204d9163f6059336b817bf8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019155"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Nosacījum access ar atbilstošu ierīci mani bloķē

**Ļoti ieteicamie rīki**

- [Ierīču reģistrācijas problēmu risinātāja rīks](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) — visaptverošs rīks, kas palīdz novērst visbiežāk sastopamās ierīču reģistrācijas problēmas.
- [Ierīču reģistrācijas savienojamības skripts —](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) rīks, kas tiek izmantots, lai nodrošinātu, ka ierīce var piekļūt ierīces reģistrācijas galapunktiem zem sistēmas konta.
- [Azure AD ierīces tīrīšanas skripts —](https://github.com/mzmaili/AzureADDeviceCleanup) rīks, kas tiek izmantots novecojušu ierīču meklēšanai un pārvaldīšanai jūsu vidē.

Tālāk ir daži bieži sastopami iemesli, kāpēc nosacījuma piekļuve var  neveiks atbilstošu ierīci vai kāpēc jūsu lietotāji saņem ziņojumu Šeit nevarat saņemt organizācijas resursa pierakstīšanās pieprasījuma laikā.

1. **Ierīce nav vajadzīgajā ierīces stāvoklī ar MDM:**

Pārbaudiet, vai ierīce ir reģistrēta pie apstiprināta MDM nodrošinātāja, piemēram, Intune, un *atzīmēta kā atbilstošs.* Papildinformāciju par Intune skatiet šajā [dokumentā.](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) Lai iegūtu labāku izpratni par ierīču atbilstību un Intune, skatiet rakstu Atbilstības politikas izmantošana, lai iestatītu kārtulas ierīcēm, kuras [pārvaldāt, izmantojot Intune](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started). Ja rodas problēmas saistībā ar ierīces reģistrāciju vietnē Intune, problēmu novēršanas detalizēto informāciju skatiet rakstā Problēmu novēršana saistībā ar ierīces [reģistrāciju programmā Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune). Papildu Intune atbalsta dienestam izveidojiet atbalsta pieprasījumu. Lai to izdarītu, apmeklējiet [Intune palīdzības un atbalsta lapu.](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport)

2. **Ierīce nav pievienota organizāciju tīklam:**

Lai piekļūtu organizācijas resursiem, ierīcei ir jābūt savienotai ar organizācijas tīklu, izmantojot tiešu savienojumu vai virtuālu privāto tīklu (VPN) un arī pievienojoties lokālajam vai Azure Active Directory. Lai pievienotos darba ierīcei organizācijas tīklā, skatiet [rakstu Pievienošanās darba ierīcei savas organizācijas tīklā.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network) Lai reģistrētu personisko/BYOD ierīci, skatiet [rakstu Personiskās ierīces](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network)reģistrēšana organizācijas tīklā.

- Lai pārbaudītu, vai ierīce ir pievienojusi savienojumu tīklam, varat izpildīt darbības reģistrētajām ierīcēm [šeit](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) vai darba [ierīcēm šeit.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined) Lai problēmu noteiktu organizācijas tīkla savienojamībā, izpildiet tālāk norādītās vadlīnijas.

    1. Pierakstieties pakalpojumā Windows, izmantojot savu darba vai mācību kontu, piemēram, alain@contoso.com.
    2. Savienošana uz organizācijas tīklu, izmantojot VPN vai DirectAccess.
    3. Kad ir izveidots savienojums, nospiediet taustiņu kombināciju **Windows logotipa taustiņš+L,** lai bloķētu ierīci.
    4. Atbloķējiet ierīci, izmantojot savu darba vai mācību kontu, un pēc tam mēģiniet vēlreiz piekļūt problemātiskai programmai vai pakalpojumam.

Ja redzat **kļūdas ziņojumu Vairs nevarat šeit no šīs** vietas, problēma, visticamāk, ir citā vietā.

3. **Operētājsistēma netiek atbalstīta:**

Pārliecinieties, vai izmantojat atbalstītu operētājsistēmas versiju, tostarp:

- **Windows klients: Windows** 7 vai jaunāka versija

- **Windows Serveris:** Windows Server 2008 R2 vai jaunāka versija

- **macOS:** macOS X vai jaunāka versija

- **Android un iOS:** Android un iOS mobilo operētājsistēmu jaunākā versija

4. **Tīmekļa pārlūkprogramma netiek atbalstīta:**

Tālāk, lūdzu, atrodiet atbalstītās pārlūkprogrammas. Lai iegūtu Chrome atbalstu Windows versiju 1703 vai jaunāku versiju, Windows 10 nepieciešams konta paplašinājums. Ja ierīcē ir instalēta programma Edge 85+, lietotājam ir jāveic pierakstīšanās, lai pareizi nodotu ierīces atbilstības informāciju. Papildinformāciju skatiet [šeit.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)

- **Windows 10**: Microsoft Edge, Internet Explorer, Chrome
- **Windows 8/8.1:** Internet Explorer, Chrome
- **Windows 7:** Internet Explorer, Chrome
- **iOS:** Microsoft Edge, Intune managed browser, Safari
- **Android:** **Microsoft Edge**: Intune pārvaldīta pārlūkprogramma, Chrome
- **Windows Phone**: Microsoft Edge, Internet Explorer
- **Windows Server 2019:** Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016:** Internet Explorer
- **Windows Server 2012 R2:** Internet Explorer
- **Windows Server 2008 R2:** Internet Explorer
- **macOS**: Chrome, Safari

Papildinformāciju par **ziņojumu un problēmu novēršanas darbībām** skatiet [šeit.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation)
