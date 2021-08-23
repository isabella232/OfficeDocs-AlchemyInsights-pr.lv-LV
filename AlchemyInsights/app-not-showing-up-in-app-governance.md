---
title: Programmu pārvaldības lietojumprogrammas netiek rādītas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12734"
ms.openlocfilehash: a8d176fdee073e41b61de6f53c728601da955aaa
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/16/2021
ms.locfileid: "58454695"
---
# <a name="my-app-isnt-showing-up-in-app-governance"></a>Programmu pārvaldības lietojumprogrammas netiek rādītas

Ja jūsu lietojumprogramma netiek rādīta programmu pārvaldībā, pārbaudiet tālāk norādītos.

1. Dodieties [uz Azure AD](https://aad.portal.azure.com/) un atrodiet savas lietojumprogrammas ID, lapas Pārskats augšējā joslā meklējot lietojumprogrammas nosaukumu.

1. Access Graph Explorer un meklējiet lietojumprogrammas ID pakalpojuma pamatnosaukā, izmantojot šo vaicājumu un aizstājot ar atbilstošo programmas <appId> ID: < https://graph.microsoft.com/v1.0/servicePrincipals? $search= "appId: <appId> ">

1. Ja netiek atgriezti rezultāti, meklējiet programmas ID lietojumprogrammā, izmantojot šo vaicājumu un aizstājot ar atbilstošo programmas <appId> ID: < https://graph.microsoft.com/v1.0/applications? $search= "appId: <appId> ">

Ja saistībā ar vaicājumu rodas problēmas, skatiet rakstu [Atbalsta saņemat.](https://docs.microsoft.com/microsoft-365/business-video/get-help-support) 

Papildinformāciju vai ieskatu par savām programmām programmu pārvaldībā skatiet rakstā [Uzziniet par redzamību un ieskatiem.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-overview)

Papildinformāciju par programmu skatīšanu skatiet rakstā [Programmu skatīšana](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-view-apps).
