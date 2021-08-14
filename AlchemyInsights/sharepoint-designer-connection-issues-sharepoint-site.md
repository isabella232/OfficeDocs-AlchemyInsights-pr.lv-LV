---
title: SharePoint Designer connection issues
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
ms.openlocfilehash: d55f7c1902bb623900fa74bdae70695b6e04ad84ce7b6ea314db614283ec436d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53942032"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer connection issues 

Ja SharePoint noformētājam ir radušās savienojuma problēmas ar SharePoint vietnēm, lūdzu, izmēģiniet tālāk norādītos bieži lietotos risinājumus.

1. darbība. Pārbaudiet, vai programma SharePoint Designer 2013 ir atjaunināta ar [SharePoint Designer 1.](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) servisa pakotni un [2016. gada 2.](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)augusta atjauninājumu pakalpojumam SharePoint Designer 2013.



2. darbība. Lokālo kešatmiņas failu notīrīšana:

1. Aizveriet SharePoint Designer 2013.

2. Lokālajā datorā noņemiet visus failus, kas atrodas katrā no tālāk redzamajām mapēm.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Atveriet SharePoint Designer 2013 un vēlreiz ievadiet kontu, lai redzētu, vai tas darbojas.

3. [darbība. Modernās autentifikācijas iespējošana Office 2013 Windows ierīcēs.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)

4. darbība. Administratoriem ir vajadzēs atļaut pielāgotu skriptu SharePoint administrēšanas centra iestatījumos, lai ļautu izveidot SharePoint Designer savienojumu.  [Papildinformāciju skatiet rakstā Pielāgota skripta atļaušana](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) vai neatļaušana.


