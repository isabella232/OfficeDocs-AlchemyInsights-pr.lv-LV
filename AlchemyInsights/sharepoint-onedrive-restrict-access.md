---
title: Piekļuves ierobežošana koplietošanas vidē SharePoint vai pakalpojumā OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700462"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Piekļuves ierobežošana koplietošanas vidē SharePoint vai pakalpojumā OneDrive

Pastāv vairāki veidi, kā ierobežot piekļuvi pakalpojumam SharePoint Online/OneDrive pakalpojumiem. Tālāk ir minētas dažādas pieejas ierobežojumu metodes. 

**Atļauju ierobežojums**

Pakalpojumā SharePoint Online un OneDrive darbam mēs ierobežojam piekļuvi tādiem vienumiem kā vietnes, faili un mapes, piešķirot piekļuvi tikai tām grupām/personām, kurām ir jābūt piekļuvei.

- [SharePoint saraksta vai bibliotēkas atļauju pielāgošana](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [SharePoint vietnes atļauju pielāgošana](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Atļauju maiņa apakšmapē](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Piekļuves kontrolēšana no nepārvaldītām ierīcēm](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Kā SharePoint vai globālais administrators varat bloķēt vai ierobežot piekļuvi SharePoint un OneDrive saturam no nepārvaldītām ierīcēm (kas nav hibrīda reklāma un nav saderīga ar Intune).

**Tīkla atrašanās vietas ierobežojums**

Kā IT administrators varat kontrolēt piekļuvi SharePoint un OneDrive resursiem, pamatojoties uz noteiktām tīkla vietām, kurām uzticaties. To sauc arī par atrašanās vietu. Lai iegūtu papildinformāciju, skatiet rakstu [piekļuves kontrolēšana SharePoint Online un OneDrive datiem, pamatojoties uz tīkla atrašanās vietu](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Vietnes bloķēšanas ierobežojums** 

Pakalpojumā SharePoint Online jums ir iespēja bloķēt vietņu kolekciju, līdz ar to nevienam nav piekļuves. To iestata, izmantojot PowerShell un [SharePoint Online pārvaldības čaulu](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) , izmantojot [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState rekvizītu.

**Lietotāju ierobežošana, lai izveidotu vietnes vai apakšvietnes**

Kā SharePoint administrators vai globālais administrators varat ļaut lietotājiem izveidot un pārvaldīt savas SharePoint vietnes, noteikt, kādas vietnes var izveidot un norādīt vietņu atrašanās vietu. Lai iegūtu papildinformāciju, lūdzu, skatiet rakstu [vietņu izveides pārvaldība pakalpojumā SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

