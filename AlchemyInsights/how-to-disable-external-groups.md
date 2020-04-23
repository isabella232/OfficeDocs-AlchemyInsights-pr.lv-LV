---
title: Kā atspējot ārējās grupas
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 2159feb4aa3999072de57d76790a2959c7355976
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720775"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="23825-102">Kā atspējot ārējās grupas</span><span class="sxs-lookup"><span data-stu-id="23825-102">How to disable External Groups</span></span>

<span data-ttu-id="23825-103">Yammer ārējā ziņojumapmaiņa attiecas Exchange transporta kārtulas (ETRs), preventīvā kontrole, lai novērstu uzņēmuma informācijas koplietošanas.</span><span class="sxs-lookup"><span data-stu-id="23825-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="23825-104">Lai aizliegtu lietotājiem izveidot ārēju grupu, ir jākonfigurē Exchange transporta kārtulu (ETR) un pēc tam jākonfigurē Yammer izmantot Exchange transporta kārtulu bloķēt ārējo ziņojumapmaiņu.</span><span class="sxs-lookup"><span data-stu-id="23825-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="23825-105">Kad esat izveidojis kārtulu Exchange Online administrēšanas centrs, veiciet tālāk norādītās darbības, lai iestatītu ETR pieteikties Yammer:</span><span class="sxs-lookup"><span data-stu-id="23825-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="23825-106">Piesakieties Yammer kā pārbaudīts admin un **Yammer administrēšanas centrs**, dodieties uz C \*\* \> satura un drošības drošības iestatījumus.\*\*</span><span class="sxs-lookup"><span data-stu-id="23825-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="23825-107">Sadaļā **ārējā ziņojumapmaiņa**atlasiet **ieviest Exchange Online Exchange transporta kārtulas (ETRs) Yammer.**</span><span class="sxs-lookup"><span data-stu-id="23825-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="23825-108">Izvēlieties **saglabāt**.</span><span class="sxs-lookup"><span data-stu-id="23825-108">Choose **Save**.</span></span>

<span data-ttu-id="23825-109">Lai iegūtu papildinformāciju, skatiet [ārējās ziņojumapmaiņas atspējošana Yammer tīklā](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="23825-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  