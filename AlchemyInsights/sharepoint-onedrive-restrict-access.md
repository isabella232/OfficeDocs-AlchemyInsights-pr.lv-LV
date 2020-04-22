---
title: Piekļuves ierobežošana programmā SharePoint vai OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 39aa8cd6e649eca4a1e196eeb589a825364d0977
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692772"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Piekļuves ierobežošana programmā SharePoint vai OneDrive

Ir vairāki veidi, kā ierobežot piekļuvi SharePoint Online/OneDrive pakalpojumiem. Šīs dažādās pieejas ierobežošanas metodes ir izklāstītas turpmāk. 

**Atļauju ierobežojums**

SharePoint Online un OneDrive uzņēmumiem, mēs ierobežojam piekļuvi tādiem vienumiem kā vietnes, faili un mapes, piešķirot piekļuvi tikai tām grupām/personām, kurām ir jābūt piekļuvei.

- [Atļauju pielāgošana SharePoint sarakstam vai bibliotēkai](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [SharePoint vietnes atļauju pielāgošana](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Mainīt atļaujas apakšmapē](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Piekļuves kontrole no nepārvaldītām ierīcēm](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

SharePoint vai globālā administrēšanas, varat bloķēt vai ierobežot piekļuvi SharePoint un OneDrive saturu no nepārvaldīts ierīces (kas nav hibrīds AD pievienojās vai atbilst InTune).

**Tīkla atrašanās vietas ierobežojums**

Kā IT administrators varat kontrolēt piekļuvi SharePoint un OneDrive resursiem, pamatojoties uz definētajām tīkla vietām, kurām uzticaties. Šī ir pazīstama arī kā politika, kuras pamatā ir atrašanās vieta. Lai iegūtu papildinformāciju, lūdzu, skatiet [piekļuves kontrole SharePoint Online un OneDrive datus, pamatojoties uz tīkla atrašanās vietu](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Vietnes bloķēšanas ierobežojums** 

Programmā SharePoint Online jums ir iespēja bloķēt vietņu kolekciju, tāpēc nevienam nav piekļuves. Tas ir iestatīts, izmantojot PowerShell un [SharePoint Online pārvaldības čaulu](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) , izmantojot rekvizītu [Set sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate.

**Aizliegt lietotājiem veidot vietnes vai apakšvietnes**

Kā SharePoint administrēšanas vai globālās administrēšanas lietotāji var ļaut lietotājiem izveidot un pārvaldīt savas SharePoint vietnes, noteikt, kāda veida vietnes viņi var izveidot, un norādīt vietņu atrašanās vietu. Lai iegūtu papildinformāciju, lūdzu, skatiet [pārvaldīt vietnes izveide SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

