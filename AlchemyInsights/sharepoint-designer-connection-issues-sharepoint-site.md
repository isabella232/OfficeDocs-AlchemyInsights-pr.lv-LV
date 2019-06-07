---
title: SharePoint Online atļauju līmeņus
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760699"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer savienojuma problēmas 

Ja SharePoint Designer radušās savienojuma problēmas SharePoint vietnēm, lūdzu, mēģiniet šādus kopīgus risinājumus.

1. darbība: Pārliecinieties, vai SharePoint Designer tiek atjaunināts.

- [SharePoint Designer 2013.](https://www.microsoft.com/download/details.aspx?id=35491)

- [SharePoint Designer 1. servisa pakotne (SP1)](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [Atjauninājums programmai SharePoint Designer 2013 (KB3114721)](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

2. solis: Notīrīt lokālajā kešatmiņā failus

- Tuvu SharePoint Designer 2013.

- Lokālajā datorā, dodieties uz šīm mapēm, lai dzēstu kešatmiņā failus.

- Noklikšķiniet uz Sākt, palaist, kā _ arī izdzēst visus failus atrast katrā no vietām zemāk.

%AppData%\Microsoft\Web servera Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

Atveriet SharePoint Designer 2013 un ievadiet kontu vēlreiz, lai redzētu, vai tas darbojas.

3. solis: [Iespējot mūsdienu biroja 2013 ierīcēs, izmantojot Windows autentifikāciju](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)

4. solis: Administratoriem būs nepieciešams pielāgots skripts ļauj atļaut savienojumu SharePoint Designer.

Detalizētām darbībām, piemērus un apsvērumi sk [Atļaut vai aizliegt pielāgotu skriptu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


