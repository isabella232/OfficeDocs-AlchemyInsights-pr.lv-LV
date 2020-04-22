---
title: Piekļuve liegta, skatot darbplūsmu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: c576bf88225582f2577e0b59506a7482cf9f38d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687337"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="7be54-102">Piekļuve liegta, skatot darbplūsmu</span><span class="sxs-lookup"><span data-stu-id="7be54-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="7be54-103">SharePoint 2013 darbplūsmas, kas mēģina nosūtīt e-pasta ziņojumu SharePoint grupai var neizdoties "piekļuve liegta" kļūdas ziņojums, ja SharePoint grupas dalība nav iestatīta uz visiem.</span><span class="sxs-lookup"><span data-stu-id="7be54-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="7be54-104">**Lai novērstu šo problēmu, rīkojieties šādi:**</span><span class="sxs-lookup"><span data-stu-id="7be54-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="7be54-105">Ļaut visiem skatīt SharePoint grupas dalībniekus.</span><span class="sxs-lookup"><span data-stu-id="7be54-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="7be54-106">Noņemiet SharePoint grupu no e-pasta ziņojuma rindiņā Kam vai kopija.</span><span class="sxs-lookup"><span data-stu-id="7be54-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="7be54-107">Tieši pievienot lietotājus rindiņā Kam vai kopija, ja dalības redzamību nevar mainīt SharePoint grupai.</span><span class="sxs-lookup"><span data-stu-id="7be54-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="7be54-108">Lai skatītu plašāku informāciju, lūdzu, skatiet [http nesankcionētu uz/_vti_bin/Client.SVC/SP.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="7be54-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  