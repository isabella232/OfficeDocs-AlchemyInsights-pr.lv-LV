---
title: SharePoint Designer savienojuma problēmas
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 1d3f6ad3128292a9dbcc46cc7da23af59a63fbb4
ms.sourcegitcommit: a285c609319ade038461e090e14a701830031825
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840558"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer savienojuma problēmas 

Ja SharePoint Designer radušās savienojuma problēmas SharePoint vietnēm, lūdzu, izmēģiniet šādus risinājumus, kopīgi.

1. darbība: Pārliecinieties, ka SharePoint Designer 2013 tiek papildināta ar [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) un [2 augusts 2016 atjaunināt SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



2. solis: Notīrīt lokālajā kešatmiņā failus:

1. Tuvu SharePoint Designer 2013.

2. Lokālajā datorā noņemtu visus failus, kas atrodas katrā no šīm mapēm.

    - %AppData%\Microsoft\Web server Extensions\Cache
    - %AppData%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Atveriet SharePoint Designer 2013 un ievadiet kontu vēlreiz, lai redzētu, vai tas darbojas.

3. solis: [Iespējot mūsdienu biroja 2013 ierīcēs, izmantojot Windows autentifikāciju](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

4. solis: Administratoriem būs nepieciešams **Pielāgots skripts ļauj** SharePoint administrēšanas centru iestatījumos atļaut savienojumu SharePoint Designer. Sk [Atļaut vai aizliegt pielāgots skripts](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) plašāku informāciju.


