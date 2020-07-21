---
title: Viens lietotājs neredz pievienojumprogrammas programmā Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197963"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>Viens lietotājs neredz pievienojumprogrammas programmā Outlook

Lietotājs var būt daļa no lomas, kas nav pareizo AppsForOfficeEnabled parametru. Palaidiet šo cmdlet, lai uzzinātu, vai pareizā loma ir saistīta ar lietotāju:

Get-ManagementRoleAssignment -RoleAssignee -user@domain.com deleg $falseating | Formatēt tabulu-automātiskā loma,RoleAssigneeName,RoleAssigneeType

Papildinformāciju skatiet sadaļā To [administratoru un lietotāju nosaukājums, kuri var instalēt un pārvaldīt pievienojumprogrammas programmai Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).
