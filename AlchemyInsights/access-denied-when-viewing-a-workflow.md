---
title: Liegta piekļuve, skatot darbplūsmas
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 43369c600687d6ac253f70a8535dc2bd0d41687e
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/12/2019
ms.locfileid: "29918835"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="a9251-102">Liegta piekļuve, skatot darbplūsmas</span><span class="sxs-lookup"><span data-stu-id="a9251-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="a9251-103">Mēģinājums nosūtīt e-pastu SharePoint grupas SharePoint 2013 darbplūsmas ar kļūdas ziņojumu "Piekļuve liegta" var neizdoties, ja SharePoint grupas sastāvs nav iestatīta lietošanai ikvienam.</span><span class="sxs-lookup"><span data-stu-id="a9251-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="a9251-104">**Lai atrisinātu šo problēmu, veiciet šādas darbības:**</span><span class="sxs-lookup"><span data-stu-id="a9251-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="a9251-105">Atļaut visiem skatīt SharePoint grupas dalībnieku.</span><span class="sxs-lookup"><span data-stu-id="a9251-105">Allow everybody to see the members of the SharePoint group.</span></span> 
  
 2. <span data-ttu-id="a9251-106">Noņemtu SharePoint grupas no, kam vai kopija līniju e-pastu.</span><span class="sxs-lookup"><span data-stu-id="a9251-106">Remove the SharePoint group from the To or CC line of the email.</span></span> 
  
 3. <span data-ttu-id="a9251-107">Tieši uz Kam vai Kopija pievienojiet lietotājus rindā ja dalības redzamību nevar mainīt SharePoint grupai.</span><span class="sxs-lookup"><span data-stu-id="a9251-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span> 
  
<span data-ttu-id="a9251-108">Lai skatītu sīkāku informāciju skatiet [HTTP Unauthorized uz /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="a9251-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  

