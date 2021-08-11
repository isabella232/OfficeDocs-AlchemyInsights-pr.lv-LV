---
title: IRM konfigurācijas pārbaude jaunām OME iespējām
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12428"
- "9000078"
ms.openlocfilehash: 62697d6379ea6ab3c6af86d3bab752af560da7c1250e5ef6dd2a3eae8023a05e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812439"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>IRM konfigurācijas pārbaude jaunām OME iespējām

Lai pārbaudītu, vai jūsu Microsoft 365 nomnieks ir konfigurēts izmantot jaunās OME iespējas, izpildiet šīs cmdlet, kamēr ir izveidots [savienojums Exchange Online PowerShell:](/powershell/exchange/exchange-online-powershell)


1. Pārbaudiet sava nomnieka IRM konfigurāciju, palaižot `Get-IRMConfiguration` . Pārliecinieties, vai šīs vērtības ir **iestatītas kā Patiesas:**
    
    **Iekšējā licencēšanaEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. Izmantojot savu domēnu, sūtītāja adresi un adresātu, palaidiet `Test-IRMConfiguration` . Ja pārbaude netiek veikta, izpētiet IRM konfigurāciju.

Papildinformāciju par IRM konfigurācijas verifikāciju skatiet rakstā [Jaunas OME konfigurācijas pārbaude Exchange Online PowerShell.](/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell)