---
title: Ar VPN saistītās problēmas
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
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555234"
---
# <a name="vpn-related-issues"></a>Ar VPN saistītās problēmas

Veiksmīga VPN savienojamības implementēšana attiecībā uz MDM klientiem ir atkarīga no izvietotā profila, kas pareizi atbilst VPN infrastruktūras prasībām. Atbilstošos iestatījumus klientu platformām, kuras izmeklējat, skatiet: 

[Windows 10 un Windows Hologrāfiskās ierīces iestatījumi, lai pievienotu VPN savienojumus, izmantojot Intune](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[VPN iestatījumu pievienošana iOS un iPadOS ierīcēs programmā Microsoft Intune](https://docs.microsoft.com/intune/vpn-settings-ios)  
[Android ierīces iestatījumi VPN konfigurēšanai Intune](https://docs.microsoft.com/intune/vpn-settings-android)  
[VPN iestatījumu pievienošana macOS ierīcēs programmā Microsoft Intune](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

Ja jūsu VPN profils izmanto autentifikāciju, kuras pamatā ir sertifikāts, pārliecinieties, vai saknes sertifikāts un klienta autentifikācijas sertifikātu profili, kas saistīti ar VPN profilu, ir sekmīgi izvietoti.

**Biežāk sastopamās problēmas**

**Esmu izvietojis VPN profilu ierīcē. Intune rāda, ka tas ir izdevies, taču ierīce neveido savienojumu ar VPN.**

Veiksmīgs statuss nozīmē, ka Intune ir sekmīgi izvietojusi profilu kā konfigurētu. Tomēr šīs konfigurācijas var nesaskanēt ar jūsu tīkla un/vai autentifikācijas prasībām. Pārskatiet žurnālus infrastruktūras un autentifikācijas pakalpojumā (VPN serverī un NPS/rādiusa serverī), lai iegūtu papildinformāciju par mēģinājumu savienojumu. Lai apkopotu un pārskatītu žurnālus, jums, iespējams, būs jāstrādā ar tīkla infrastruktūras grupu vai trešās puses VPN piegādātāju.

**Konfigurējot pielāgoto VPN for iOS, programmas VPN līdzeklis nav pieejams.**

Katras lietojumprogrammas VPN iOS ierīcēm sistēmā Intune pašlaik ir pieejama konkrētam pakalpojumu sniedzēju un partneru sarakstam, kam ir jāatbilst sertifikāta priekšnosacījumiem, pirms konfigurējot vienu lietojumprogrammu VPN. Lai iegūtu papildinformāciju, skatiet rakstu [programmas Virtual Private Network (VPN) iestatīšana darbam ar iOS/iPadOS ierīcēm pakalpojumā Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app). 

Lai iegūtu papildinformāciju par visiem VPN savienojumu veidiem sistēmā Intune, skatiet rakstu [VPN profilu izveide, lai izveidotu savienojumu ar VPN serveriem Intune](https://docs.microsoft.com/intune/vpn-settings-configure).  

**pēc tam, kad tiek atvērts konfigurēts domēns, iOS pēc pieprasījuma VPN netiek aktivizēta**

Lai pārbaudītu automātiskos VPN iestatījumus, iestatiet tālāk norādītās vērtības.

Vēlos veikt šādas darbības: **katra savienojuma izveides mēģinājuma novērtēšana** 

Izvēlieties, vai veidot savienojumu: **nepieciešamības gadījumā izveidot** savienojumu

Kad lietotāji piekļūst šiem domēniem: **mērķis** *domēna nosaukums*

Ja iepriekš norādītā konfigurācija nav sekmīga, pievienojiet šādu elementu:

Ja šis vietrādis URL nav sasniedzams, pievienojiet VPN: **BADURL**