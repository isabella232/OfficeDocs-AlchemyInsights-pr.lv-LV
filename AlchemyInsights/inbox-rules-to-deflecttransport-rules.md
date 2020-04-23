---
title: 929 iesūtnes kārtulas deflectTransport noteikumi
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "929"
- "1800021"
ms.assetid: 9733ef4e-db8d-4345-a072-c251480875a1
ms.openlocfilehash: 6b6e64c0332a579e8f6132b08f2f89b15eb4de27
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43724599"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a><span data-ttu-id="7e682-102">Pasta plūsmas noteikumi (zināmi arī kā transportēšanas noteikumi)</span><span class="sxs-lookup"><span data-stu-id="7e682-102">Mail flow rules (also known as transport rules)</span></span>

- <span data-ttu-id="7e682-103">Vispārīga pasta plūsmas kārtulu pārskats: [pasta plūsmas kārtulas (transporta kārtulas) Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span><span class="sxs-lookup"><span data-stu-id="7e682-103">General overview of mail flow rules: [Mail flow rules (transport rules) in Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span></span>

- <span data-ttu-id="7e682-104">Iestatīšana pasta plūsma kārtulas: [pasta plūsma kārtulu procedūras Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span><span class="sxs-lookup"><span data-stu-id="7e682-104">Setup mail flow rules: [Mail flow rule procedures in Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span></span>

- <span data-ttu-id="7e682-105">Pasta plūsmas kārtulu izveide, modificēšana un dzēšana: [pasta plūsmas kārtulu pārvaldīšana](https://technet.microsoft.com/library/jj657505.aspx)</span><span class="sxs-lookup"><span data-stu-id="7e682-105">Create, modify, and delete mail flow rules: [Manage mail flow rules](https://technet.microsoft.com/library/jj657505.aspx)</span></span>

<span data-ttu-id="7e682-106">Varat arī pārvaldīt pasta plūsmas kārtulas Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="7e682-106">You can also manage mail flow rules in Exchange Online PowerShell.</span></span> <span data-ttu-id="7e682-107">Lai iegūtu papildinformāciju, skatiet [Get transportrule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (skatīt), [jauna transportrule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (izveidot), [Noņemt Transportrule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (dzēst), [Set Transportrule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (modificēt esošo), [atspējojiet TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (atspējot esošo) un [Iespējot transportrule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (iespējot esošo).</span><span class="sxs-lookup"><span data-stu-id="7e682-107">For more information, see [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (view), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (create), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (delete), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (modify existing), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (disable existing), and [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (enable existing).</span></span>

<span data-ttu-id="7e682-108">Papildu pasta plūsma kārtula cmdlet: [Get TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (saraksts pieejamās darbības), [saņemt Transportrulepredikāts](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (saraksts pieejamie nosacījumi un izņēmumi), [eksporta transportrulecollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (eksporta noteikumi) un [Import-transportrulecollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (importa noteikumi).</span><span class="sxs-lookup"><span data-stu-id="7e682-108">Additional mail flow rule cmdlets: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (list available actions), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (list available conditions and exceptions), [Export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (export rules), and [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (import rules).</span></span>
