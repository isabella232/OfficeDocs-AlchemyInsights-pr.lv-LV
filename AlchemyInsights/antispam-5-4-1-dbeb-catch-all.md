---
title: Pretsurogātpasta 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717368"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="22ec0-102">Piegādes problēmu novēršana kļūdas kodam 550 5.4.1 relay piekļuvei</span><span class="sxs-lookup"><span data-stu-id="22ec0-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="22ec0-103">Šī problēma rodas, [pārbaudot, vai e-pasta adrese ir derīga, lai neļautu bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) , kad ievadāt Microsoft tīklu.</span><span class="sxs-lookup"><span data-stu-id="22ec0-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="22ec0-104">Izmēģiniet kādu no tālāk norādītajām darbībām.</span><span class="sxs-lookup"><span data-stu-id="22ec0-104">Try the following:</span></span>

1. <span data-ttu-id="22ec0-105">Noteikt, vai problēma ir saistīta ar visu domēnu vai vienu e-pasta adresi:</span><span class="sxs-lookup"><span data-stu-id="22ec0-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="22ec0-106">Viss domēns: dažreiz domēns ir jāsinhronizē. mēģiniet [Iestatīt domēnu uz iekšējs un pēc tam atpakaļ uz autoritatīvo](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="22ec0-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="22ec0-107">Viena e-pasta adrese: dažreiz adrese ir jāsinhronizē. var palīdzēt mainīt SMTP starpniekservera adresi un pēc tam to mainīt atpakaļ.</span><span class="sxs-lookup"><span data-stu-id="22ec0-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="22ec0-108">Noteikt, vai problēma ir specifiska grupai vai publiskai mapei.</span><span class="sxs-lookup"><span data-stu-id="22ec0-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="22ec0-109">Dažiem objektu veidiem objekti, iespējams, ir manuāli jāveido Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="22ec0-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="22ec0-110">Ja jums ir vajadzīgas papildu palīdzība, lūdzu, atveriet atbalsta biļeti un norādiet problēmas apjomu (ieskaitot tā objekta tipu, ko sūtāt), lai mēs varētu jums palīdzēt labāk.</span><span class="sxs-lookup"><span data-stu-id="22ec0-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>