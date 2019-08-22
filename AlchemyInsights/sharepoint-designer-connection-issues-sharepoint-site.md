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
ms.openlocfilehash: a4aeaeaea5743c276b907c78317ff30f5610be81
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/22/2019
ms.locfileid: "36508430"
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


