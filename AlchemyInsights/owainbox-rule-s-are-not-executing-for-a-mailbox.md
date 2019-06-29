---
title: 1332 OWA - iesūtnes kārtula ir nav izpildes pastkastes
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 7d1848830847fc6722da20e09a4875f49bf02bd3
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/28/2019
ms.locfileid: "35360924"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="3e5b1-102">Iesūtnes kārtulas nedarbojas, kā paredzēts</span><span class="sxs-lookup"><span data-stu-id="3e5b1-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="3e5b1-103">Pārbaudiet šos iestatījumus:</span><span class="sxs-lookup"><span data-stu-id="3e5b1-103">Verify the following settings:</span></span>

- <span data-ttu-id="3e5b1-104">Ziņojums var būt novirzīts, pārsūtīt vai atbildētu automātiski, pamatojoties uz iesūtnes kārtulas tikai vienu reizi.</span><span class="sxs-lookup"><span data-stu-id="3e5b1-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="3e5b1-105">Novirzot kārtulu (iesūtnes kārtulu vai pasta plūsmas kārtula, pazīstams arī kā transporta kārtulu) var ne vairāk kā desmit pāradresācijas adresātu pievienošana ziņojumam.</span><span class="sxs-lookup"><span data-stu-id="3e5b1-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="3e5b1-106">Papildinformāciju skatiet šeit: [Journal, transporta un iesūtnes kārtulu robežas](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="3e5b1-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="3e5b1-107">Iesūtnes kārtulas nedarbojas uz alternatīvo journaling pastkasti.</span><span class="sxs-lookup"><span data-stu-id="3e5b1-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="3e5b1-108">Papildinformāciju par alternatīvo journaling pastkasti, skatiet [alternatīvo journaling pastkastes](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="3e5b1-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="3e5b1-109">Lai novērstu šo problēmu, skatiet [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="3e5b1-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="3e5b1-110">Ja iepriekšējie jautājumi neatbilst, palaidiet iesūtnes kārtulu diagnostikas pārskata pirms jūs izskatīt šo problēmu ar Microsoft Support:</span><span class="sxs-lookup"><span data-stu-id="3e5b1-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="3e5b1-111">Atvērt šo pastkasti programmā Outlook Web un noklikšķiniet uz **Iestatījumi** \> **Opcijas** \> **organizēt e-pastu** \> **Iesūtnes kārtulas**.</span><span class="sxs-lookup"><span data-stu-id="3e5b1-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>

2. <span data-ttu-id="3e5b1-112">Lapas apakšdaļā noklikšķiniet uz **Ja kārtulas nedarbojas klikšķi šeit diagnostikas atskaites ģenerēšanai**.</span><span class="sxs-lookup"><span data-stu-id="3e5b1-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
