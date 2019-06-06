---
title: Ierobežot piekļuvi SharePoint vai OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 5101366ff65f477c19b9c7f2c0d7065cf88501b0
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/05/2019
ms.locfileid: "34735149"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Ierobežot piekļuvi SharePoint vai OneDrive

Ir daudzi veidi, kā ierobežot piekļuvi SharePoint Online/OneDrive pakalpojumus. Šīs dažādās piekļuves ierobežošanas metodes ir izklāstīti turpmāk. 

Ierobežot atļaujas

SharePoint Online un OneDrive uzņēmējdarbībai, mums ierobežot piekļuvi precēm, piemēram, vietnēm, failus un mapes tikai piešķirot piekļuvi šīm grupām/personām, vajadzētu būt pieejamai.

[Pielāgot SharePoint saraksta vai bibliotēkas atļauju](https://support.office.com/en-us/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

[Pielāgot SharePoint vietnes atļaujas](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions)

[Mainīt atļaujas apakšmapi](https://support.office.com/en-us/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

[No nepārvaldītiem ierīču piekļuves kontrole](https://docs.microsoft.com/en-us/sharepoint/control-access-from-unmanaged-devices)

Kā SharePoint vai globālās administrēšanas Office 365, var bloķēt vai ierobežot piekļuvi SharePoint un OneDrive saturu no nepārvaldītiem ierīču (tām nav hibrīds AD pievienojās vai atbilstošu Intune).

Tīkla atrašanās vietas ierobežojums

Kā IT administrators, jūs varat kontrolēt piekļuvi SharePoint un OneDrive resursus, balstoties uz noteiktiem tīkla vietas, kurām uzticaties. Tas ir arī pazīstams kā politikas atkarībā no atrašanās vietas. Plašāku informāciju skatiet [SharePoint Online un OneDrive datus, pamatojoties uz tīkla atrašanās vietas piekļuves kontrole](https://docs.microsoft.com/en-us/sharepoint/control-access-based-on-network-location)

Bloķēt vietnes ierobežojumu 

Programmā SharePoint Online, jums ir iespēja, lai bloķētu vietņu kolekciju, lai nevienam nav piekļuves. Tas tiek iestatīts, izmantojot PowerShell un [SharePoint Online Management Shell](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) , izmantojot [Set-SPOSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) - LockState īpašumu.

Aizliegtu lietotājiem veidot vietnes vai apakšvietņu

Kā SharePoint administrēšanas vai Office 365 globālās administrēšanas, jūs varat ļaut lietotājiem izveidot un administrēt savas SharePoint vietnes, nosakiet, kāda veida portālos tie var radīt, un norādiet vietnes atrašanās vietu. Plašāku informāciju skatiet [Manage vietņu izveide SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/manage-site-creation)

