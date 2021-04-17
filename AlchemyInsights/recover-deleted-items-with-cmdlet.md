---
title: Izdzēsto vienumu atkopšana, izmantojot cmdlet
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
- "1800008"
- "5718"
ms.openlocfilehash: d8f2a50f39d7bcd321692ab093e2efa6613e9814
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835818"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="65e37-102">Izdzēsto vienumu atkopšana, izmantojot cmdlet</span><span class="sxs-lookup"><span data-stu-id="65e37-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="65e37-103">Izmantojiet cmdlet [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps), lai skatītu pastkastēs izdzēstos vienumus.</span><span class="sxs-lookup"><span data-stu-id="65e37-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="65e37-104">Kad izdzēstie vienumi ir atrasti, izmantojiet cmdlet [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps), lai tos atjaunotu.</span><span class="sxs-lookup"><span data-stu-id="65e37-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="65e37-105">Pilnu detalizēto informāciju skatiet aprakstā par [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="65e37-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="65e37-106">Lai varētu palaist šo cmdlet, jums ir jābūt piešķirtai pastkastes importēšanas/eksportēšanas lomai.</span><span class="sxs-lookup"><span data-stu-id="65e37-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="65e37-107">Papildinformāciju skatiet aprakstā par [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="65e37-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
