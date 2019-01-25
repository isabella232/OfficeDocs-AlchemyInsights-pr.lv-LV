---
title: 1554 Winsock kļūda 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 96a9cfd11941158ddf13655c74974e3eb800e570
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/24/2019
ms.locfileid: "29479505"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="22a7a-102">Winsock kļūda 10061</span><span class="sxs-lookup"><span data-stu-id="22a7a-102">Winsock error 10061</span></span>

<span data-ttu-id="22a7a-p101">Šo kļūdas kodu, nozīmē, ka Office 365 nevarētu izveidot TCP ligzda (savienojums) ar mērķa resursdatoru. Visdrīzāk, ka cēlonis šīs kļūdas ir ar ugunsmūra konfigurāciju saistīta problēma. Lai novērstu problēmu, pārbaudiet šos iestatījumus:</span><span class="sxs-lookup"><span data-stu-id="22a7a-p101">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host. The most likely cause of this error is a problem with your firewall configuration. To fix the problem, check these settings:</span></span>
  
- <span data-ttu-id="22a7a-106">Pārbaudiet, vai jūsu ugunsmūra konfigurēšanu ar informāciju, kas atrodas [Office 365 URL un IP adrešu diapazons](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="22a7a-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>
    
- <span data-ttu-id="22a7a-107">Ja kļūda ir specifiski uz Exchange Online aizsardzība (EOP), jums vajadzētu ir iepriekš paziņots [Exchange Online aizsardzība IP adreses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)maiņa.</span><span class="sxs-lookup"><span data-stu-id="22a7a-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
    
- <span data-ttu-id="22a7a-108">Pārliecinieties, ka jūsu interneta pakalpojumu sniedzēja (ISP) nav bloķē portu.</span><span class="sxs-lookup"><span data-stu-id="22a7a-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>
    
- <span data-ttu-id="22a7a-109">Pārbaudiet, vai gudrs uzņēmējas un mērķa servera uzstādījumus jūsu savienotāji.</span><span class="sxs-lookup"><span data-stu-id="22a7a-109">Verify the smart host and target server settings in your connectors.</span></span>
    
<span data-ttu-id="22a7a-110">Ievērojiet, ka Office 365 nav bloķēt *ienākošos* savienojumus šādā veidā.</span><span class="sxs-lookup"><span data-stu-id="22a7a-110">Note that Office 365 doesn't block  *incoming*  connections in this manner.</span></span> 
  

