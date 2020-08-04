---
title: Intune Wi-Fi profili
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555313"
---
# <a name="intune-wi-fi-profiles"></a>Intune Wi-Fi profili

Veiksmīga Wi-Fi savienojamības ar MDM klientiem ieviešana ir atkarīga no pareiza izvietošanas profila, kas atbilst korporatīvās Wi-Fi infrastruktūras prasībām. Lai pārskatītu atbilstošos iestatījumus klientu platformām, kuras izmeklējat, skatiet: 

[Wi-Fi iestatījumu pievienošana ierīcēs, kurās darbojas Android programmā Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android)

[Wi-Fi iestatījumu pievienošana Android Enterprise atvēlētajām un pilnībā pārvaldītajām ierīcēm pakalpojumā Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[Wi-Fi iestatījumu pievienošana operētājsistēmā iOS un iPadOS ierīcēs programmā Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[Wi-Fi iestatījumu pievienošana sistēmai Windows 10 un jaunākām ierīcēm pakalpojumā Intune](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[Wi-Fi iestatījumu importēšana Windows ierīcēs Intune](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**Biežāk sastopamās problēmas**

**Esmu izvietojis Wi-Fi profilu, kas ir atkarīgs no Wi-Fi profilā norādītā izvietotā sertifikāta. Taču konfigurācijas profiliem tiek rādīts kļūdas statuss.**

Pārbaudiet, vai jūsu ierīce saņēma sertifikātu.

1. Sistēmā Intune dodieties uz **visas ierīces** un atlasiet ierīci, > **ierīces konfigurāciju**.

2. Pārbaudiet, vai visi gaidītie profili ir uzskaitīti un darbojas veiksmīgi.

3. Android profilam, ja jums ir starpposma sertifikāti jūsu sertifikātu ķēdē, pārliecinieties, vai tie ir izvietoti Android ierīcēs.

    Lai pārbaudītu sertifikāta statusu, dodieties uz **ierīču konfigurācijas**  >  **profili**  >  **Android Intermediate CA**  >  **Rekvizīti**  >  **uzticams sertifikāts**.

Ja joprojām redzat kļūdas, pārskatiet sadaļu procedūras un problēmu novēršanas darbības. Papildinformāciju skatiet rakstā [pārskats par problēmu novēršanas SCEP sertifikātu profiliem ar Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).

**Es Izvietoju Wi-Fi profilu ierīcē. Intune rāda, ka tas ir izdevies, taču ierīce neveido savienojumu ar Wi-Fi.**

Veiksmīgs statuss nozīmē, ka Intune ir sekmīgi izvietojusi profilu kā konfigurētu. Tomēr šīs konfigurācijas var nesaskanēt ar jūsu tīkla un/vai autentifikācijas prasībām. Lai iegūtu detalizētu informāciju par mēģinājumu savienojumu, pārskatiet žurnālus infrastruktūras un autentifikācijas pakalpojumos (Wi-Fi piekļuves punkta kontrollerī un NPS/rādiusa serverī). Lai apkopotu un pārskatītu žurnālus, jums, iespējams, būs jāstrādā ar tīkla infrastruktūras grupu vai trešās puses Wi-Fi piegādātāju.