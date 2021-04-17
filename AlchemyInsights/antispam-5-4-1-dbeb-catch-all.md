---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821454"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="48a5d-102">Piegādes problēmu (kļūdas kods 550 5.4.1 pārraide liegta) novēršana</span><span class="sxs-lookup"><span data-stu-id="48a5d-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="48a5d-103">Šī problēma rodas, [pārbaudot, vai](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) e-pasta adrese ir derīga, lai novērstu atlēcienu rādīšanu Microsoft tīklā.</span><span class="sxs-lookup"><span data-stu-id="48a5d-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="48a5d-104">Veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="48a5d-104">Try the following:</span></span>

1. <span data-ttu-id="48a5d-105">Nosakiet, vai problēma ir raksturīga visam domēnam vai vienai e-pasta adresei:</span><span class="sxs-lookup"><span data-stu-id="48a5d-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="48a5d-106">Viss domēns: dažreiz domēns ir jāsinhronizē; mēģiniet [iestatīt domēnu uz Iekšējs un pēc tam atpakaļ uz Autoritatīvs](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="48a5d-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="48a5d-107">Viena e-pasta adrese: dažreiz adrese ir jāsinhronizē; smtp starpniekservera adreses maiņa un pēc tam atpakaļadreses maiņa var palīdzēt.</span><span class="sxs-lookup"><span data-stu-id="48a5d-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="48a5d-108">Nosakiet, vai problēma ir specifiska grupai vai publiskai mapei.</span><span class="sxs-lookup"><span data-stu-id="48a5d-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="48a5d-109">Dažu objektu tipu gadījumā objektus var būt nepieciešams manuāli izveidot pakalpojumā Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="48a5d-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="48a5d-110">Ja jums nepieciešama papildu palīdzība, lūdzu, atveriet atbalsta biļeti un norādiet problēmas tvērumu (tostarp tā objekta veidu, uz kuru nosūtāt), lai mēs varētu jums palīdzēt labāk.</span><span class="sxs-lookup"><span data-stu-id="48a5d-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>