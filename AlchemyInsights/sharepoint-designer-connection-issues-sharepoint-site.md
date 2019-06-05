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
ms.openlocfilehash: 7451cfe957545537298f57feb5b47bd6d43cddbf
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716898"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer savienojuma problēmas 

<p>Ja SharePoint Designer radušās savienojuma problēmas SharePoint vietnēm, lūdzu, mēģiniet šādus kopīgus risinājumus.</p> <p><strong>1. solis:</strong> <strong>Atjaunināšanas pārliecinieties, vai SharePoint Designer&nbsp; </strong></p> <ul> <li><a href="https://www.microsoft.com/en-us/download/details.aspx?id=35491">SharePoint Designer 2013.</a></li> <li><a href="https://support.microsoft.com/en-us/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1">SharePoint Designer 1. servisa pakotne (SP1)</a></li> <li><a href="https://support.microsoft.com/en-us/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721">Atjauninājums programmai SharePoint Designer 2013 (KB3114721)</a></li> </ul> <p><strong>2. solis:</strong> <strong>Notīrīt lokālajā kešatmiņā failus</strong>&nbsp;</p> <ol> <li style="font-weight: 400;">Tuvu SharePoint Designer 2013.&nbsp;</li> <li style="font-weight: 400;">Lokālajā datorā, dodieties uz šīm mapēm, lai dzēstu kešatmiņā failus.&nbsp;</li> <li style="font-weight: 400;">Noklikšķiniet uz <strong>Start -&gt; palaist</strong> un dzēsiet visus failus, kas atrada zem katra no zemāk atrašanās vietas.&nbsp;<br /><br />%AppData%\Microsoft\Web server Extensions\Cache<br />%AppData%\Microsoft\SharePoint Designer\ProxyAssemblyCache<br />%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</li> <li style="font-weight: 400;">Atveriet SharePoint Designer 2013 un ievadiet kontu vēlreiz, lai redzētu, vai tas darbojas.</li> </ol> <p><strong>3. solis:</strong> <a href="https://docs.microsoft.com/en-us/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=%252fen-us%252farticle%252fEnable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&amp;view=o365-worldwide">, <strong>Iespējot mūsdienu biroja 2013 ierīcēs, izmantojot Windows autentifikāciju</strong></a>&nbsp;</p> <p><strong>4. solis:</strong> <strong>Administratoriem būs nepieciešams atļaut pielāgoto skriptu, lai SharePoint Designer savienojumu</strong>.</p> <p>Detalizētām darbībām, piemērus un apsvērumi sk <a href="https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script">Atļaut vai aizliegt pielāgotu skriptu</a>.&nbsp;</p>


