---
title: Jūsu arhīva pastkaste ir gandrīz pilna
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974407"
---
# <a name="your-archive-mailbox-is-almost-full"></a><span data-ttu-id="77a30-102">Jūsu arhīva pastkaste ir gandrīz pilna</span><span class="sxs-lookup"><span data-stu-id="77a30-102">Your archive mailbox is almost full</span></span>

<span data-ttu-id="77a30-103">Ja lietotājs saņem brīdinājumu; **Jūsu arhīva pastkaste ir gandrīz pilna** vai ir jāpalielina savas arhīva pastkastes lielums, šeit sniegti daži padomi.</span><span class="sxs-lookup"><span data-stu-id="77a30-103">If the user receives the warning; **Your archive mailbox is almost full**, or you need to increase the size of their archive mailbox, here are some tips:</span></span>

1. <span data-ttu-id="77a30-104">Ja lietotājam ir piešķirts Exchange Online 1. plāns, jauniniet uz **Exchange Online 2. plānu** , lai palielinātu lielumu no 50 GB līdz 100gb.</span><span class="sxs-lookup"><span data-stu-id="77a30-104">If the user is assigned an Exchange Online Plan 1, upgrade to **Exchange Online Plan 2** license to increase the size from 50 GB to 100GB.</span></span>
1. <span data-ttu-id="77a30-105">Ja lietotājam jau ir piešķirts kāds no šiem: **Exchange Online 2. plāns** vai Exchange Online 1. plāns ar Exchange Online arhivēšanas pievienojumprogrammu, veiciet tālāk norādītās darbības, lai iespējotu automātisko arhivēšanu.</span><span class="sxs-lookup"><span data-stu-id="77a30-105">If the user is already assigned either of the following: **Exchange Online Plan 2** or an Exchange Online Plan 1 with an Exchange Online Archiving add-on, use the steps below to enable Auto-Expanding archiving:.</span></span>
 
    1. <span data-ttu-id="77a30-106">[Savienojuma izveide ar Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="77a30-106">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span></span>
    2. <span data-ttu-id="77a30-107">Palaidiet tālāk norādīto unifiedgroup lietotājam.  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span><span class="sxs-lookup"><span data-stu-id="77a30-107">Run the following commandlet for the user:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span></span>
    1. <span data-ttu-id="77a30-108">Palaidiet tālāk norādīto unifiedgroup, lai pārliecinātos, vai tas ir iespējots lietotājam.  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span><span class="sxs-lookup"><span data-stu-id="77a30-108">Run the following commandlet to confirm it is enabled for the user:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span></span>

<span data-ttu-id="77a30-109">Papildinformāciju skatiet rakstā:</span><span class="sxs-lookup"><span data-stu-id="77a30-109">For more information see:</span></span>

- [<span data-ttu-id="77a30-110"> Iespējot neierobežotu arhivēšanu — administrēšanas palīdzība — Microsoft 365 atbilstība | Microsoft dokumenti</span><span class="sxs-lookup"><span data-stu-id="77a30-110"> Enable unlimited archiving - Admin Help - Microsoft 365 Compliance | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [<span data-ttu-id="77a30-111">Exchange Online ierobežojumi — pakalpojumu apraksti | Microsoft dokumenti</span><span class="sxs-lookup"><span data-stu-id="77a30-111">Exchange Online limits - Service Descriptions | Microsoft Docs</span></span>](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [<span data-ttu-id="77a30-112">Jaunināšana uz citu biznesa plānu | Microsoft dokumenti</span><span class="sxs-lookup"><span data-stu-id="77a30-112">Upgrade to a different business plan | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

