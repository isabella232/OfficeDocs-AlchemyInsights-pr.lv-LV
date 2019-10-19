---
title: Piekļuves ierobežošana programmā SharePoint vai OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bef0612903b9bb455aa34e90d35d6b7b9093b4e0
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/18/2019
ms.locfileid: "36750671"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Piekļuves ierobežošana programmā SharePoint vai OneDrive

Ir vairāki veidi, kā ierobežot piekļuvi SharePoint Online/OneDrive pakalpojumiem. Šīs dažādās pieejas ierobežošanas metodes ir izklāstītas turpmāk. 

**Atļauju ierobežojums**

SharePoint Online un OneDrive uzņēmumiem, mēs ierobežojam piekļuvi tādiem vienumiem kā vietnes, faili un mapes, piešķirot piekļuvi tikai tām grupām/personām, kurām ir jābūt piekļuvei.

- [Atļauju pielāgošana SharePoint sarakstam vai bibliotēkai](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [SharePoint vietnes atļauju pielāgošana](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Mainīt atļaujas apakšmapē](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Piekļuves kontrole no nepārvaldītām ierīcēm](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

SharePoint vai globālās administrēšanas Office 365, varat bloķēt vai ierobežot piekļuvi SharePoint un OneDrive saturu no nepārvaldīts ierīces (kas nav hibrīds AD pievienojās vai atbilst InTune).

**Tīkla atrašanās vietas ierobežojums**

Kā IT administrators varat kontrolēt piekļuvi SharePoint un OneDrive resursiem, pamatojoties uz definētajām tīkla vietām, kurām uzticaties. Šī ir pazīstama arī kā politika, kuras pamatā ir atrašanās vieta. Lai iegūtu papildinformāciju, lūdzu, skatiet [piekļuves kontrole SharePoint Online un OneDrive datus, pamatojoties uz tīkla atrašanās vietu](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Vietnes bloķēšanas ierobežojums** 

Programmā SharePoint Online jums ir iespēja bloķēt vietņu kolekciju, tāpēc nevienam nav piekļuves. Tas ir iestatīts, izmantojot PowerShell un [SharePoint Online pārvaldības čaulu](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) , izmantojot rekvizītu [Set sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate.

**Aizliegt lietotājiem veidot vietnes vai apakšvietnes**

Kā SharePoint admin vai Office 365 globālais administrators varat ļaut lietotājiem izveidot un pārvaldīt savas SharePoint vietnes, noteikt, kādas vietnes viņi var izveidot, un norādīt vietņu atrašanās vietu. Lai iegūtu papildinformāciju, lūdzu, skatiet [pārvaldīt vietnes izveide SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

