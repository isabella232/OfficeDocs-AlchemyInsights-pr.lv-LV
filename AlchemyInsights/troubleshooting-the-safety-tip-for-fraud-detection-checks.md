---
title: Drošības padoma novēršana krāpšanas atklāšanas pārbaužu gadījumā
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834738"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="cd031-102">Drošības padoma novēršana krāpšanas atklāšanas pārbaužu gadījumā</span><span class="sxs-lookup"><span data-stu-id="cd031-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="cd031-103">Ja saņemat drošības padomu, kas vēsta "Sūtītājs neizdevās veikt krāpšanas atklāšanas pārbaudes un var nebūt tas, kas izskatās pēc", sūtītājam neizdevās nodot DKIM vai SPF autentifikācijas pārbaudes.</span><span class="sxs-lookup"><span data-stu-id="cd031-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="cd031-104">Vislabākais veids, kā šo problēmu atrisināt, ir atļaut sūtītājam sevi autorizēt.</span><span class="sxs-lookup"><span data-stu-id="cd031-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="cd031-105">Ja sūtītājs sūta ziņojumu jūsu vārdā, jums tie ir jāpilnvaro, pievienojot sūtītāja IP adresi savam SPF ierakstam.</span><span class="sxs-lookup"><span data-stu-id="cd031-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="cd031-106">[Papildinformāciju skatiet rakstā Sarkanā (aizdomīgā)](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) drošības padoma problēmu novēršana attiecībā uz krāpšanas noteikšanu.</span><span class="sxs-lookup"><span data-stu-id="cd031-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="cd031-107">Lūk, dažas citas saites, kas var palīdzēt:</span><span class="sxs-lookup"><span data-stu-id="cd031-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="cd031-108">Kā Microsoft izmanto sūtītāja politikas struktūru (SPF), lai novērstu izlikšanās</span><span class="sxs-lookup"><span data-stu-id="cd031-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="cd031-109">SPF iestatīšana, lai palīdzētu novērst izlikšanās</span><span class="sxs-lookup"><span data-stu-id="cd031-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
