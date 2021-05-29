---
title: Exchange Online PowerShell mikro aiztures vai ierobežošana
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702133"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="ba1da-102">Exchange Online PowerShell mikro aiztures vai ierobežošana</span><span class="sxs-lookup"><span data-stu-id="ba1da-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="ba1da-103">Palaižot skriptus vai komandlietotnes Exchange Online, jums var tikt parādīts paziņojums “Piemērotas mikro aiztures” vai piemērota ierobežošana.</span><span class="sxs-lookup"><span data-stu-id="ba1da-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="ba1da-104">Lūk, daži ieteikumi, kā to novērst:</span><span class="sxs-lookup"><span data-stu-id="ba1da-104">Here are a few suggestions how to solve this:</span></span>

- <span data-ttu-id="ba1da-105">Lūdzu, palaidiet mūsu diagnostiku, lai atslābtu nomnieka PowerShell ierobežošanas politikas.</span><span class="sxs-lookup"><span data-stu-id="ba1da-105">Please run our diagnostics to relax your tenant's PowerShell throttling policies.</span></span> <span data-ttu-id="ba1da-106">Šis risinājums atrisinās problēmu lielākajai daļai.</span><span class="sxs-lookup"><span data-stu-id="ba1da-106">This solution will solve the problem for most.</span></span>
- <span data-ttu-id="ba1da-107">Ja problēmu joprojām nevar atrisināt, izmantojiet [Exchange Online v2 PowerShell](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)moduli, kurā iekļauti CMDlets, kuru pamatā ir REST API un kuri ir ievērojami efektīvāki.</span><span class="sxs-lookup"><span data-stu-id="ba1da-107">If issue still not solved, use the [Exchange Online v2 PowerShell module](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="ba1da-108">Šis varētu būt lielisks risinājums daudzām bieži izmantotām Get- komandlietotnēm.</span><span class="sxs-lookup"><span data-stu-id="ba1da-108">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="ba1da-109">Ja vēlaties izmantot CMDlets, kas nav apskatītas v2 modulī, lūdzu, skatiet rakstu [PowerShell cmdlet](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)izpildīšana lielam lietotāju skaitam programmā Office 365, kurā ir ietvertas sarunas par PowerShell ierobežošanas ierobežojumu apiet Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="ba1da-109">If you need to use CMDlets that are not covered in the v2 module, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around PowerShell throttling limits in Exchange Online.</span></span>
