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
ms.openlocfilehash: 680df9e6e2404ff6b60b17d6ac88e202e9a7bb25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830040"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="11e95-102">Exchange Online PowerShell mikro aiztures vai ierobežošana</span><span class="sxs-lookup"><span data-stu-id="11e95-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="11e95-103">Palaižot skriptus vai komandlietotnes Exchange Online, jums var tikt parādīts paziņojums “Piemērotas mikro aiztures” vai piemērota ierobežošana.</span><span class="sxs-lookup"><span data-stu-id="11e95-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="11e95-104">Tālāk ir sniegti divi ieteikumi par to:</span><span class="sxs-lookup"><span data-stu-id="11e95-104">Here are two suggestions related to this:</span></span>

- <span data-ttu-id="11e95-105">Iespējams, ka vēlaties izmēģināt [Exchange Online v2 PowerShell moduli](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), kas iekļauj komandlietotnes, kas ir balstītas uz REST API un tām ir būtiski lielāka veiktspēja.</span><span class="sxs-lookup"><span data-stu-id="11e95-105">You might want to try using the [Exchange Online v2 PowerShell module](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="11e95-106">Šis varētu būt lielisks risinājums daudzām bieži izmantotām Get- komandlietotnēm.</span><span class="sxs-lookup"><span data-stu-id="11e95-106">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="11e95-107">Ja jums ir jāizmanto komandlietotnes, kas vēl nav iekļautas v2 modulī, lūdzu, lasiet [PowerShell komandlietotņu palaišana lielam Office 365 lietotāju skaitam](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), kur ir aprakstīts risinājums PowerShell ierobežojumu apiešanai pakalpojumā Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="11e95-107">If you need to use CMDlets that are not covered in the v2 module yet, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around expected PowerShell throttling limits in Exchange Online.</span></span>
