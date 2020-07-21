---
title: Vairāki lietotāji neredz pievienojumprogrammas programmā Outlook
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
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197978"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Vairāki lietotāji neredz pievienojumprogrammas programmā Outlook

Ja kā pirmo problēmu novēršanas darbību tiek pārbaudītas Outlook pievienojumprogrammas un neviena no tām nav parādīta, izmantojiet **cmdlet Get-OrganizationConfig** PowerShell, lai vaicātu _parametru AppsForOfficeEnabled._ Ja vaicājums atgriež vērtību False , **iestatiet**šo parametru **uz True,** izmantojot cmdlet **Set-OrganizationConfig,** tāpēc pievienojumprogrammas tiek parādītas, kā paredzēts.

Nav ieteicams, ka _AppsForOfficeEnabled parametrs_ ir iestatīts uz **False**. False vērtība **ignorē** visus iepriekš administratīvo un lietotāju lomu iestatījumus un neļauj jaunas programmas aktivizē jebkurš lietotājs organizācijā.

Papildinformāciju skatiet sadaļā To [administratoru un lietotāju nosaukāk, kuri var instalēt un pārvaldīt pievienojumprogrammas programmai Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).