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
# <a name="troubleshooting-ediscovery-holds-errors"></a><span data-ttu-id="f060a-102">Ediscovery problēmu novēršana ietver kļūdas</span><span class="sxs-lookup"><span data-stu-id="f060a-102">Troubleshooting ediscovery holds errors</span></span>

<span data-ttu-id="f060a-103">Vai radušās problēmas ar e-datu atklāšanas aizturēšanu?</span><span class="sxs-lookup"><span data-stu-id="f060a-103">Experiencing issues with eDiscovery holds?</span></span> <span data-ttu-id="f060a-104">Lūk, dažas labākās prakses piemēri:</span><span class="sxs-lookup"><span data-stu-id="f060a-104">Here are some best practices to consider:</span></span>

- <span data-ttu-id="f060a-105">Pārbaudiet aizturēšanas adresātu statusu.</span><span class="sxs-lookup"><span data-stu-id="f060a-105">Check the hold distribution status.</span></span>  <span data-ttu-id="f060a-106">Ja statuss ir **Ieslēgts (Gaida)** vai **Izslēgts (Gaida),** gaidiet adresātu aizturēšanu, lai pabeigtu.</span><span class="sxs-lookup"><span data-stu-id="f060a-106">If status is **On (Pending)** or **Off (Pending)**, wait for hold distribution to complete.</span></span>
- <span data-ttu-id="f060a-107">Sapludiniet e-datu atklāšanu, glabājiet atjauninājumus vienā lielapjoma pieprasījumā, nevis atkārtoti atjauniniet politiku katrai transakcijai.</span><span class="sxs-lookup"><span data-stu-id="f060a-107">Merge eDiscovery hold updates into a single bulk request instead of updating the policy repeatedly for each transaction.</span></span>
- <span data-ttu-id="f060a-108">Izpildiet Set-CaseHoldPolicy Powershell drošības un atbilstības centra izpildiet komandu <policyname> -RetryDistribution.</span><span class="sxs-lookup"><span data-stu-id="f060a-108">Run Set-CaseHoldPolicy <policyname> -RetryDistribution in the Security and Compliance Center Powershell.</span></span> <span data-ttu-id="f060a-109">Detalizētu informāciju skatiet [rakstā Savienošana drošības & atbilstības centra PowerShell](/powershell/exchange/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="f060a-109">For details, see [Connect to Security & Compliance Center PowerShell](/powershell/exchange/connect-to-scc-powershell).</span></span>

<span data-ttu-id="f060a-110">Norādījumus, kā pārbaudīt šos iestatījumus un veikt papildu paraugpraksi, kā mazināt un novērst e-datu atklāšanas problēmas, skatiet rakstā [E-datu](/microsoft-365/compliance/hold-distribution-errors)atklāšanas problēmu novēršana ietver kļūdas .</span><span class="sxs-lookup"><span data-stu-id="f060a-110">For steps to check these settings and additional best practices for mitigating and resolving eDiscovery holds issues, see [Troubleshoot eDiscovery hold errors](/microsoft-365/compliance/hold-distribution-errors).</span></span>
<span data-ttu-id="f060a-111">Informāciju par citu biežāk sastopamo e-datu atklāšanas problēmu novēršanu skatiet [rakstā Biežāk sastopamo e-datu atklāšanas problēmu izpēte, problēmu novēršana un novēršana.](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)</span><span class="sxs-lookup"><span data-stu-id="f060a-111">For info about troubleshooting other common eDiscovery issues, see [Investigate, troubleshoot, and resolve common eDiscovery issues](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span></span>
