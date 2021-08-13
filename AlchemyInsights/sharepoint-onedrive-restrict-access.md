---
title: Piekļuves ierobežošana programmā SharePoint vai OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: fc6731d5a7747bb4fc8d6cef1b6ac0045d11917d7f97abbb21eea9613b1b1aa2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093840"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Piekļuves ierobežošana programmā SharePoint vai OneDrive

Pastāv vairāki veidi, kā ierobežot piekļuvi SharePoint Online/OneDrive pakalpojumiem. Šīs dažādas piekļuves ierobežojuma metodes ir aprakstītas tālāk. 

**Atļauju ierobežojums**

Pakalpojumā SharePoint Online un OneDrive darbam piekļuvi vienumiem, piemēram, vietnēm, failiem un mapēm, ierobežojam tikai piešķirot piekļuvi šīm grupām/personām, kurām jābūt piekļuves tiesībām.

- [Pielāgotas atļaujas SharePoint sarakstam vai bibliotēkai](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Vietnes SharePoint pielāgošana](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Atļauju maiņa apakšmapē](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Piekļuves kontrole no nepārvaldītām ierīcēm](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Kā SharePoint globālais administrators varat bloķēt vai ierobežot piekļuvi SharePoint un OneDrive saturam no nepārvaldītām ierīcēm (tās, kas nav hibrīda AD pievienošanas vai saderīgas intune).

**Tīkla atrašanās vietas ierobežojums**

Kā IT administrators varat kontrolēt piekļuvi internetam SharePoint un OneDrive, pamatojoties uz definētām tīkla atrašanās vietām, kurām uzticaties. To sauc arī par atrašanās vietas politiku. Papildinformāciju skatiet rakstā Kā kontrolēt piekļuvi SharePoint Online un [OneDrive datiem, pamatojoties uz tīkla atrašanās vietu](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Vietņu bloķēšanas ierobežojums** 

Tīmekļa SharePoint online jums ir iespēja bloķēt vietņu kolekciju, tāpēc neviens tai nevar piekļūt. Tas tiek iestatīts, izmantojot PowerShell [un SharePoint Online pārvaldības čaulu,](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) izmantojot rekvizītu [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**Vietņu un apakšvietņu izveides ierobežošana lietotājiem**

Kā SharePoint administrators vai globālais administrators varat ļaut lietotājiem izveidot un administrēt savas SharePoint vietnes, noteikt, kādas vietnes viņi var izveidot, un norādīt vietņu atrašanās vietu. Papildinformāciju skatiet rakstā [Vietņu izveides pārvaldība programmā SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

