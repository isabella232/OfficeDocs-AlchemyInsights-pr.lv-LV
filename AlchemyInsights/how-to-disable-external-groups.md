---
title: Kā atspējot ārējo grupu
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 4683a71438ec31f9e9211404a9c66c4e45e0e1df
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/22/2019
ms.locfileid: "36540908"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="a593f-102">Kā atspējot ārējo grupu</span><span class="sxs-lookup"><span data-stu-id="a593f-102">How to disable External Groups</span></span>

<span data-ttu-id="a593f-103">Yammer ārējo ziņojumapmaiņas lieto Exchange transporta kārtulas (ETRs) kopa proaktīvas pārbaudes, lai nepieļautu uzņēmumu informāciju, neļaujot tos koplietot.</span><span class="sxs-lookup"><span data-stu-id="a593f-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="a593f-104">Lai aizliegtu lietotājiem ārējo grupu veidošanu, jums nepieciešams konfigurēt Exchange pārvadājumu noteikumu (ETR) un pēc tam konfigurējiet Yammer lietot kārtulas Exchange transports, lai bloķētu ārēja ziņojumapmaiņas.</span><span class="sxs-lookup"><span data-stu-id="a593f-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="a593f-105">Kad esat izveidojis kārtulu Exchange Online admin Center, izpildiet šos norādījumus, lai iestatītu ETR Yammer piemērot:</span><span class="sxs-lookup"><span data-stu-id="a593f-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="a593f-106">Pieteikties kā pārbaudīta admin un **Yammer administrēšanas centrs**Yammer, dodieties uz C **saturu un drošības \> drošības iestatījumus.**</span><span class="sxs-lookup"><span data-stu-id="a593f-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="a593f-107">Saskaņā ar **Ārējo ziņojumapmaiņu**, izvēlieties **realizēt jūsu Exchange Online apmaiņa transportēšanas noteikumiem (ETRs) Yammer.**</span><span class="sxs-lookup"><span data-stu-id="a593f-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="a593f-108">Izvēlieties **saglabāt**.</span><span class="sxs-lookup"><span data-stu-id="a593f-108">Choose **Save**.</span></span>

<span data-ttu-id="a593f-109">Plašāku informāciju skatiet [kontrole ārējo ziņojumapmaiņas Yammer tīklā ar Exchange pārvadāšanas noteikumiem](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="a593f-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  