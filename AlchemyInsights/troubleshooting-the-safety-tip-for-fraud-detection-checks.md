---
title: Traucējummeklēšana drošības tip par krāpšanas atklāšanas pārbaudes
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 74913492a086de688067d588e95dd87e6946743b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/02/2020
ms.locfileid: "44504990"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="c01b2-102">Traucējummeklēšana drošības tip par krāpšanas atklāšanas pārbaudes</span><span class="sxs-lookup"><span data-stu-id="c01b2-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="c01b2-103">Ja jūs saņemat drošības tip, ka saka: "sūtītājs nav mūsu krāpšanas atklāšanas pārbaudes un var nebūt, kas tie, šķiet,", tad sūtītājs neizdevās nodot vai nu DKIM vai SPF autentifikācijas pārbaudes.</span><span class="sxs-lookup"><span data-stu-id="c01b2-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="c01b2-104">Labākā metode, kā to atrisināt, ir sūtītājam autorizēt sevi.</span><span class="sxs-lookup"><span data-stu-id="c01b2-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="c01b2-105">Ja sūtītājs sūta jūsu vārdā, jums ir nepieciešams pilnvarot tos, pievienojot sūtītāja IP adresi SPF ierakstu.</span><span class="sxs-lookup"><span data-stu-id="c01b2-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="c01b2-106">Plašāku informāciju skatiet sadaļā [problēmu novēršana saistībā ar sarkano (aizdomīgo) drošības padomu par krāpšanas noteikšanas pārbaudēm](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .</span><span class="sxs-lookup"><span data-stu-id="c01b2-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="c01b2-107">Šeit ir dažas citas saites, kas var palīdzēt:</span><span class="sxs-lookup"><span data-stu-id="c01b2-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="c01b2-108">Kā Microsoft izmanto sūtītāja politikas struktūra (SPF), lai novērstu izlikšanos</span><span class="sxs-lookup"><span data-stu-id="c01b2-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="c01b2-109">Iestatīt SPF, lai palīdzētu novērst izlikšanos</span><span class="sxs-lookup"><span data-stu-id="c01b2-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
