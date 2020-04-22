---
title: AntiSpam 5.4.1 DBEB catch-visi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707918"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="0fde9-102">Izlabojiet kļūdas kods piegādes problēmas 550 5.4.1 relay piekļuve liegta</span><span class="sxs-lookup"><span data-stu-id="0fde9-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="0fde9-103">Šī problēma rodas, [pārbaudot, lai redzētu, vai e-pasta adrese ir derīga, lai novērstu atgriešanu](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) ievadot Microsoft Network.</span><span class="sxs-lookup"><span data-stu-id="0fde9-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="0fde9-104">Mēģiniet veikt šādas darbības:</span><span class="sxs-lookup"><span data-stu-id="0fde9-104">Try the following:</span></span>

1. <span data-ttu-id="0fde9-105">Nosakiet, vai problēma ir specifiska visam domēnam vai vienai e-pasta adresei:</span><span class="sxs-lookup"><span data-stu-id="0fde9-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="0fde9-106">Viss domēns: dažreiz domēns ir jāsinhronizē; mēģiniet [Iestatīt domēnu uz iekšējo un pēc tam atpakaļ uz autoritatīvu](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="0fde9-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="0fde9-107">Viena e-pasta adrese: dažreiz adrese ir jāsinhronizē; mainot SMTP starpniekservera adrese un pēc tam mainot to atpakaļ var palīdzēt.</span><span class="sxs-lookup"><span data-stu-id="0fde9-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="0fde9-108">Nosakiet, vai problēma ir saistīta ar grupu vai publisko mapi.</span><span class="sxs-lookup"><span data-stu-id="0fde9-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="0fde9-109">Dažiem objektu tipiem objekti, iespējams, ir jāizveido manuāli pakalpojumā Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0fde9-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="0fde9-110">Ja jums nepieciešama papildu palīdzība, lūdzu, atveriet atbalsta biļeti un norādiet jautājuma tvērumu (ieskaitot tā objekta veidu, uz kuru sūtāt), lai mēs varētu jums palīdzēt labāk.</span><span class="sxs-lookup"><span data-stu-id="0fde9-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>