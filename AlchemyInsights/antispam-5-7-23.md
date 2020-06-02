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
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506450"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="d7570-102">Novērst e-pasta piegādes problēmas kļūdas kods 5.7.23</span><span class="sxs-lookup"><span data-stu-id="d7570-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="d7570-103">Pārbaudiet, vai jūsu domēnam ir SPF DNS ieraksts tīmeklī publiski pieejamā SPF vai DNS ierakstu pārbaudītājā.</span><span class="sxs-lookup"><span data-stu-id="d7570-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="d7570-104">Pārbaudiet, vai izejošais ziņojums netika identificēts kā Microsoft surogātpasts un maršrutēts, izmantojot [augsta riska piegādes pūlu](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="d7570-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="d7570-105">Augsta riska piegādes pūla ziņojumi netiks iet SPF pārbaudes, un tādēļ netiks akceptēts mērķa e-pasta organizācijas.</span><span class="sxs-lookup"><span data-stu-id="d7570-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="d7570-106">Ja problēma joprojām pastāv, iespējams, vajadzēs sazināties ar administratora pasta resursdatora, kuru mēģināt nosūtīt e-pastu.</span><span class="sxs-lookup"><span data-stu-id="d7570-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="d7570-107">Pierakstiet detalizētu ārējo kļūdu, kas pieejama ziņojumā par atlēcienu.</span><span class="sxs-lookup"><span data-stu-id="d7570-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="d7570-108">Iespējams, ka Microsoft atbalsts nevarēs palīdzēt tālāk.</span><span class="sxs-lookup"><span data-stu-id="d7570-108">Microsoft support may not be able to assist further.</span></span>
