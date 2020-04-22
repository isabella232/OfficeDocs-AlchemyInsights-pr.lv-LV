---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676504"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="8940c-102">Novērst e-pasta piegādes problēmas kļūdas kods 5.7.23</span><span class="sxs-lookup"><span data-stu-id="8940c-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="8940c-103">Pārbaudiet, vai jūsu domēnam ir SPF DNS ieraksts tīmeklī publiski pieejamā SPF vai DNS ierakstu pārbaudītājā.</span><span class="sxs-lookup"><span data-stu-id="8940c-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="8940c-104">Pārbaudiet, vai izejošais ziņojums netika identificēts kā Microsoft surogātpasts un maršrutēts, izmantojot [augsta riska piegādes pūlu](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="8940c-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="8940c-105">Augsta riska piegādes pūla ziņojumi netiks iet SPF pārbaudes, un tādēļ netiks akceptēts mērķa e-pasta organizācijas.</span><span class="sxs-lookup"><span data-stu-id="8940c-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="8940c-106">Ja problēma joprojām pastāv, iespējams, vajadzēs sazināties ar administratora pasta resursdatora, kuru mēģināt nosūtīt e-pastu.</span><span class="sxs-lookup"><span data-stu-id="8940c-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="8940c-107">Pierakstiet detalizētu ārējo kļūdu, kas pieejama ziņojumā par atlēcienu.</span><span class="sxs-lookup"><span data-stu-id="8940c-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="8940c-108">Iespējams, ka Microsoft atbalsts nevarēs palīdzēt tālāk.</span><span class="sxs-lookup"><span data-stu-id="8940c-108">Microsoft support may not be able to assist further.</span></span>
