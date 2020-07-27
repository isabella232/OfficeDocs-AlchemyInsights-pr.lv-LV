---
title: Pievienojot pievienojumprogrammu programmā Outlook, vairāki lietotāji saņem piekļuves liegšanas kļūdu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424180"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Pievienojot pievienojumprogrammu programmā Outlook, vairāki lietotāji saņem piekļuves liegšanas kļūdu

Varat norādīt, kuriem jūsu organizācijas administratoriem ir atļaujas instalēt un pārvaldīt pievienojumprogrammas darbam ar Outlook. Varat arī norādīt, kuriem lietotājiem jūsu organizācijā ir atļauja instalēt un pārvaldīt pievienojumprogrammas savām vajadzībām.

Detalizētu informāciju skatiet rakstā [administratoru un lietotāju, kas var instalēt un pārvaldīt pievienojumprogrammas programmai Outlook, norādīšana](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).

Lai pārliecinātos, vai esat veiksmīgi piešķīris lietotājam atļaujas, aizstājiet <Role Name> ar tās lomas nosaukumu, ko vēlaties pārbaudīt, un izpildiet šādu komandu pakalpojumā Exchange Online PowerShell:

Get-ManagementRoleAssignment-lomai " <Role Name> "-GetEffectiveUsers

Šajā piemērā ir parādīts, kā pārbaudīt, kam ir piešķirtas atļaujas, lai instalētu pievienojumprogrammas no Office veikala organizācijai.

PowerShell

-Loma "organizācijas Marketplace lietojumprogrammas"-GetEffectiveUsers

Rezultātos Iegūstiet-ManagementRoleAssignment, pārskatiet ievadnes kolonnā efektīvie lietotāji.

Detalizētu informāciju par sintaksi un parametriem skatiet rakstā [iegūšana-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 