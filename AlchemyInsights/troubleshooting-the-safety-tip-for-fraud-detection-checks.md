---
title: Problēmu novēršanas drošības tip krāpšanas atklāšanai pārbauda
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.openlocfilehash: 24842e8cc5c6e47fb0eb637e6a3211637ede1ed8
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/15/2019
ms.locfileid: "28300753"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="1f95b-102">Problēmu novēršanas drošības tip krāpšanas atklāšanai pārbauda</span><span class="sxs-lookup"><span data-stu-id="1f95b-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="1f95b-p101">Ja jums ir iegūt drošības tip, ka saka "sūtītājs neizdevās mūsu krāpšanas atklāšanas pārbaudēm un, iespējams, kuri tie varētu būt", tad sūtītājs izturējušas DKIM vai SPF autentifikācijas pārbaudes. Labākā metode, lai atrisinātu šo problēmu, ir sūtītāja sevi autorizēšanai. Ja sūtītājs sūta jūsu vārdā, jums tos atļaut SPF ierakstu, pievienojot sūtītāja IP adrese.</span><span class="sxs-lookup"><span data-stu-id="1f95b-p101">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks. The best method to resolve this is for the sender to authorize themselves. If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="1f95b-106">Vairāk info sk [Troubleshooting sarkans (aizdomīgu) drošības tip krāpšanas atklāšanai pārbauda](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .</span><span class="sxs-lookup"><span data-stu-id="1f95b-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span> 
  
<span data-ttu-id="1f95b-107">Šeit ir dažas saites, kas var palīdzēt:</span><span class="sxs-lookup"><span data-stu-id="1f95b-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="1f95b-108">Kā Office 365 izmanto sūtītāja politikas pamatnostādnes (SPF) novērst izlikšanos</span><span class="sxs-lookup"><span data-stu-id="1f95b-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/en-us/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)
    
- [<span data-ttu-id="1f95b-109">Lai palīdzētu novērst izlikšanos, kas izveidota Office 365 SPF</span><span class="sxs-lookup"><span data-stu-id="1f95b-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/en-us/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    

