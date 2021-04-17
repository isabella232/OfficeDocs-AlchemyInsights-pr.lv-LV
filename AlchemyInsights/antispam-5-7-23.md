---
title: Pretspams - 5.7.23
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
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821418"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="4e6e3-102">E-pasta piegādes problēmu (kļūdas kods 5.7.23) novēršana</span><span class="sxs-lookup"><span data-stu-id="4e6e3-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="4e6e3-103">Pārbaudiet sava domēna SPF DNS ierakstu publiski pieejama SPF vai DNS ieraksta pārbaudītājā tīmeklī.</span><span class="sxs-lookup"><span data-stu-id="4e6e3-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="4e6e3-104">Pārbaudiet, vai korporācija Microsoft nav identificējusi izejošo ziņojumu kā surogātpastu un maršrutēta, izmantojot augsta [riska piegādes pūlu.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)</span><span class="sxs-lookup"><span data-stu-id="4e6e3-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="4e6e3-105">Ziņojumi augsta riska piegādes pūlā neiztur SPF pārbaudes, tāpēc mērķa e-pasta organizācijā tos nepieņems.</span><span class="sxs-lookup"><span data-stu-id="4e6e3-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="4e6e3-106">Ja problēma joprojām pastāv, iespējams, ir jāsazinās ar tā pasta viesošanas pakalpojumu resursdatora administratoru, kuram mēģināt nosūtīt e-pastu.</span><span class="sxs-lookup"><span data-stu-id="4e6e3-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="4e6e3-107">Pievērsiet uzmanību detalizētai ārējai kļūdai, kas pieejama atlēciena ziņojumā.</span><span class="sxs-lookup"><span data-stu-id="4e6e3-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="4e6e3-108">Iespējams, Microsoft atbalsta dienests nevarēs jums palīdzēt.</span><span class="sxs-lookup"><span data-stu-id="4e6e3-108">Microsoft support may not be able to assist further.</span></span>
