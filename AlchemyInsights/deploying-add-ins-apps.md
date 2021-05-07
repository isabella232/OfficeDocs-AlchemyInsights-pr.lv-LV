---
title: Pievienojumprogrammu izvietošana Microsoft 365 programmas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: a878a35ba9b530ce22ca7c263d20bd942d6896a8
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233541"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>Pievienojumprogrammu izvietošana Microsoft 365 programmas

Centralizētā izvietošana ir ieteicamais veids, Office pievienojumprogrammas izvietot lietotājiem un grupām jūsu organizācijā. Lai izvietotu pievienojumprogrammas, veiciet tālāk norādītās darbības.

**Piezīme.** Lai instalētu pievienojumprogrammas Office kā atsevišķs lietotājs, skatiet rakstu Pievienojumprogrammu skatīšana, pārvaldība un instalēšana [Office programmās.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d) Pārliecinieties arī par to, ka ir iespējota Office veikala pievienojumprogrammu iegāde. Detalizētu informāciju skatiet rakstā [Pievienojumprogrammu lejupielādes neļaušana, izslēdzot pievienojumprogrammu Office veikalu visos](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook)klientos (izņemot Outlook).

1. Pārliecinieties, vai jūsu vide atbilst prasībām par pievienojumprogrammu izvietošanu, izmantojot centralizēto izvietošanu. Papildinformāciju skatiet [rakstā Prasības](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).
2. Lai **izvietotu Iestatījumi,** dodieties uz sadaļu  >    >   Integrēto lietojumprogrammu iegūšana Microsoft 365 administrēšanas centrā. 

Piezīmes. 

- Integrētajām lietojumprogrammām nepieciešams, lai administratoram būtu globālā administratora Exchange administratora atļaujas.

- Izvietojot pievienojumprogrammas vairākiem lietotājiem, ieteicams piešķirt uzdevumus, izmantojot grupas, nevis atsevišķus lietotājus. Papildinformāciju [skatiet rakstā Apsvērumi par pievienojumprogrammas piešķiršanu lietotājiem un grupām.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)

- Centralizētā izvietošana neatbalsta lietotājus ligzdotās grupās vai grupās, kam ir vecākgrupas. Detalizētu informāciju skatiet rakstā [Lietotāju un grupu piešķiršana.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)

- Pārliecinieties, vai Microsoft 365 programmas pārvaldības pakalpojums (GUID: 0517ffae-825d-4aff-999e-3f2336b8a20a) ir iespējots, lai lietotāji varētu pierakstīties. Detalizētu informāciju skatiet rakstā [Programmas rekvizītu konfigurēšana.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)

- Ja, izvietojot pievienojumprogrammas, rodas problēmas, izmantojot integrētās lietojumprogrammas, mēģiniet izvietot, [izmantojot pievienojumprogrammas.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)

Papildinformāciju skatiet rakstā:

[Pievienojumprogrammu izvietošana administrēšanas centrā](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Pievienojumprogrammu pārvaldība administrēšanas centrā](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Centralizētās izvietošanas PowerShell cmdlet izmantošana pievienojumprogrammu pārvaldīšanai](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Pievienojumprogrammu Office, izmantojot centralizēto izvietošanu, izmantojot Microsoft 365 centru](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Problēmu novēršana: lietotājam netiek rādītas pievienojumprogrammas](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Ar pievienojumprogrammu Office saistīto lietotāju kļūdu novēršana](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)