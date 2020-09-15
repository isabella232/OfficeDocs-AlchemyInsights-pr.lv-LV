---
title: Kā atspējot ārējās grupas
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704135"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="4ff38-102">Kā atspējot ārējās grupas</span><span class="sxs-lookup"><span data-stu-id="4ff38-102">How to disable External Groups</span></span>

<span data-ttu-id="4ff38-103">Yammer ārējā ziņojumapmaiņa lieto Exchange pārvadāšanas kārtulas (ETRs) — proaktīvu vadīklu kopu, kas neļauj koplietot uzņēmuma informāciju.</span><span class="sxs-lookup"><span data-stu-id="4ff38-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="4ff38-104">Lai lietotājiem ierobežotu iespēju izveidot ārējas grupas, ir jākonfigurē Exchange transporta kārtula (ETR lietošanai) un pēc tam jākonfigurē Yammer, lai izmantotu Exchange transporta kārtulu, lai bloķētu ārējo ziņojumapmaiņu.</span><span class="sxs-lookup"><span data-stu-id="4ff38-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="4ff38-105">Kad esat izveidojis kārtulu Exchange Online administrēšanas centrā, veiciet tālāk norādītās darbības, lai iestatītu ETR lietošanai lietošanai pakalpojumā Yammer.</span><span class="sxs-lookup"><span data-stu-id="4ff38-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="4ff38-106">Piesakieties pakalpojumā Yammer kā verificēts administrators un **Yammer administrēšanas centrā**dodieties uz C **satura un drošības \> drošības iestatījumi.**</span><span class="sxs-lookup"><span data-stu-id="4ff38-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="4ff38-107">Sadaļā **ārējā ziņojumapmaiņa**atlasiet **ieviest savas Exchange Online Exchange transporta kārtulas (ETRs) pakalpojumā Yammer.**</span><span class="sxs-lookup"><span data-stu-id="4ff38-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="4ff38-108">Izvēlieties **Saglabāt**.</span><span class="sxs-lookup"><span data-stu-id="4ff38-108">Choose **Save**.</span></span>

<span data-ttu-id="4ff38-109">Papildinformāciju skatiet rakstā [ārējas ziņojumapmaiņas atspējošana Yammer tīklā](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="4ff38-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  