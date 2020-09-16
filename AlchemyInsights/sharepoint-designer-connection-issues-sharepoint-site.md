---
title: SharePoint Designer savienojuma problēmas
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727178"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer savienojuma problēmas 

Ja programmā SharePoint Designer ir radušās savienojuma problēmas ar SharePoint vietnēm, izmēģiniet šos bieži izmantotos risinājumus.

1. darbība: Pārbaudiet, vai SharePoint Designer 2013 ir atjaunināts, izmantojot [SharePoint Designer 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) . un [2016 2. augusta SharePoint Designer 2013 atjauninājumu](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



2. darbība: notīriet lokālos kešatmiņas failus:

1. SharePoint Designer 2013.

2. Lokālajā datorā noņemiet visus failus, kas atrasti katrā no šīm mapēm.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Atveriet SharePoint Designer 2013 un vēlreiz ievadiet kontu, lai uzzinātu, vai tas darbojas.

3. darbība: [modernās autentifikācijas iespējošana sistēmai Office 2013 Windows ierīcēs](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

4. darbība: administratoriem ir **jāatļauj pielāgot skriptu** SharePoint administrēšanas centra iestatījumos, lai atļautu SharePoint Designer savienojumu. Papildinformāciju skatiet rakstā [pielāgota skripta atļaušana vai novēršana](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .


