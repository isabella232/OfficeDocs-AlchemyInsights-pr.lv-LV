---
title: 1332 OWA - iesūtnes kārtula ir nav izpildes pastkastes
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1332
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: c0b221b5335254bd0f1eb4b258efa6946376ca12
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/13/2019
ms.locfileid: "31858751"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="2794b-102">Iesūtnes kārtulas nedarbojas, kā paredzēts</span><span class="sxs-lookup"><span data-stu-id="2794b-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="2794b-103">Pārbaudiet šos iestatījumus:</span><span class="sxs-lookup"><span data-stu-id="2794b-103">Verify the following settings:</span></span>

- <span data-ttu-id="2794b-104">Ziņojums var būt novirzīts, pārsūtīt vai atbildētu automātiski, pamatojoties uz iesūtnes kārtulas tikai vienu reizi.</span><span class="sxs-lookup"><span data-stu-id="2794b-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="2794b-105">Novirzot kārtulu (iesūtnes kārtulu vai pasta plūsmas kārtula, pazīstams arī kā transporta kārtulu) var ne vairāk kā desmit pāradresācijas adresātu pievienošana ziņojumam.</span><span class="sxs-lookup"><span data-stu-id="2794b-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="2794b-106">Papildinformāciju skatiet šeit: [Journal, transporta un iesūtnes kārtulu robežas](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="2794b-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="2794b-107">Iesūtnes kārtulas nedarbojas uz alternatīvo journaling pastkasti.</span><span class="sxs-lookup"><span data-stu-id="2794b-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="2794b-108">Papildinformāciju par alternatīvo journaling pastkasti, skatiet [alternatīvo journaling pastkastes](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="2794b-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="2794b-109">Lai novērstu šo problēmu, skatiet [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="2794b-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="2794b-110">Ja iepriekšējie jautājumi neatbilst, palaidiet iesūtnes kārtulu diagnostikas pārskata pirms jūs izskatīt šo problēmu ar Microsoft Support:</span><span class="sxs-lookup"><span data-stu-id="2794b-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="2794b-111">Atvērt šo pastkasti programmā Outlook Web un noklikšķiniet uz **Iestatījumi** \> **Opcijas** \> **organizēt e-pastu** \> **Iesūtnes kārtulas**.</span><span class="sxs-lookup"><span data-stu-id="2794b-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>

2. <span data-ttu-id="2794b-112">Lapas apakšdaļā noklikšķiniet uz **Ja kārtulas nedarbojas klikšķi šeit diagnostikas atskaites ģenerēšanai**.</span><span class="sxs-lookup"><span data-stu-id="2794b-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
