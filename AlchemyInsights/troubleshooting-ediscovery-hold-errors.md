---
title: Ediscovery problēmu novēršana ietver kļūdas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676275"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a>Ediscovery problēmu novēršana ietver kļūdas

Vai radušās problēmas ar e-datu atklāšanas aizturēšanu? Lūk, dažas labākās prakses piemēri:

- Pārbaudiet aizturēšanas adresātu statusu.  Ja statuss ir **Ieslēgts (Gaida)** vai **Izslēgts (Gaida),** gaidiet adresātu aizturēšanu, lai pabeigtu.
- Sapludiniet e-datu atklāšanu, glabājiet atjauninājumus vienā lielapjoma pieprasījumā, nevis atkārtoti atjauniniet politiku katrai transakcijai.
- Izpildiet Set-CaseHoldPolicy Powershell drošības un atbilstības centra izpildiet komandu <policyname> -RetryDistribution. Detalizētu informāciju skatiet [rakstā Savienošana drošības & atbilstības centra PowerShell](/powershell/exchange/connect-to-scc-powershell).

Norādījumus, kā pārbaudīt šos iestatījumus un veikt papildu paraugpraksi, kā mazināt un novērst e-datu atklāšanas problēmas, skatiet rakstā [E-datu](/microsoft-365/compliance/hold-distribution-errors)atklāšanas problēmu novēršana ietver kļūdas .
Informāciju par citu biežāk sastopamo e-datu atklāšanas problēmu novēršanu skatiet [rakstā Biežāk sastopamo e-datu atklāšanas problēmu izpēte, problēmu novēršana un novēršana.](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)
