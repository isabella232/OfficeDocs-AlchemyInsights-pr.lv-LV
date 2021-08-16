---
title: Satura meklēšana nav rezultātu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: b53534dd0666fa64e692910aa6800abab30169a97fbe567c815ce6b948381a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058009"
---
# <a name="no-results-from-content-searchexports"></a>Nav rezultātu no satura meklēšanas/eksportēšanas

Problēmas ar satura meklēšanu/eksportēšanu neatgriež nekādus datus, iespējams, izraisa konkrēts administrators iestatīts atbilstības drošības filtrs, kas netika darīts zināmu visiem administratoriem.

Lai novērstu šo problēmu, pārbaudiet, vai ir kāds atbilstības drošības filtrs, kas varētu izraisīt šo problēmu:
1. Savienošana uz drošības un atbilstības centra Powershell
2. Palaidiet šādus komandsīklietotņus:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter organizācijas $org