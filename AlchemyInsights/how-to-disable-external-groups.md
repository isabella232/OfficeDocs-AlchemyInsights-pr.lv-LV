---
title: Kā atspējot ārējo grupu
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 4d911c319c3e8e327f9b3af3ba67816e646bc468
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/23/2019
ms.locfileid: "32399670"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="6f8d1-102">Kā atspējot ārējo grupu</span><span class="sxs-lookup"><span data-stu-id="6f8d1-102">How to disable External Groups</span></span>

<span data-ttu-id="6f8d1-103">Yammer ārējo ziņojumapmaiņas lieto Exchange transporta kārtulas (ETRs) kopa proaktīvas pārbaudes, lai nepieļautu uzņēmumu informāciju, neļaujot tos koplietot.</span><span class="sxs-lookup"><span data-stu-id="6f8d1-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="6f8d1-104">Lai aizliegtu lietotājiem ārējo grupu veidošanu, jums nepieciešams konfigurēt Exchange pārvadājumu noteikumu (ETR) un pēc tam konfigurējiet Yammer lietot kārtulas Exchange transports, lai bloķētu ārēja ziņojumapmaiņas.</span><span class="sxs-lookup"><span data-stu-id="6f8d1-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span> 
  
<span data-ttu-id="6f8d1-105">Kad esat izveidojis kārtulu Exchange Online admin Center, izpildiet šos norādījumus, lai iestatītu ETR Yammer piemērot:</span><span class="sxs-lookup"><span data-stu-id="6f8d1-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="6f8d1-106">Pieteikties kā pārbaudīta admin un **Yammer administrēšanas centrs**Yammer, dodieties uz C **ontent un drošības \> drošības iestatījumus.**</span><span class="sxs-lookup"><span data-stu-id="6f8d1-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **ontent and Security \> Security Settings.**</span></span>
    
- <span data-ttu-id="6f8d1-107">Saskaņā ar **Ārējo ziņojumapmaiņu**, izvēlieties **realizēt jūsu Exchange Online apmaiņa transportēšanas noteikumiem (ETRs) Yammer.**</span><span class="sxs-lookup"><span data-stu-id="6f8d1-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>
    
- <span data-ttu-id="6f8d1-108">Izvēlieties **Saglabāt**.</span><span class="sxs-lookup"><span data-stu-id="6f8d1-108">Choose **Save**.</span></span> 
    
<span data-ttu-id="6f8d1-109">Plašāku informāciju skatiet [kontrole ārējo ziņojumapmaiņas Yammer tīklā ar Exchange pārvadāšanas noteikumiem](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="6f8d1-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  

