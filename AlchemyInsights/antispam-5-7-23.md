---
title: Antispam-5.7.23
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
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717332"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="f5761-102">E-pasta piegādes problēmu (kļūdas kods 5.7.23) novēršana</span><span class="sxs-lookup"><span data-stu-id="f5761-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="f5761-103">Pārbaudiet sava domēna SPF DNS ierakstu par publiski pieejamu SPF vai DNS ierakstu pārbaudītāju tīmeklī.</span><span class="sxs-lookup"><span data-stu-id="f5761-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="f5761-104">Pārliecinieties, ka korporācija Microsoft nav identificējusi izejošo ziņojumu kā surogātpastu un maršrutēja [lielu riska piegādes pūlu](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="f5761-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="f5761-105">Ziņojumi augsta riska piegādes pūlā neveic SPF pārbaudes, tāpēc galamērķa e-pasta organizācija nepieņems.</span><span class="sxs-lookup"><span data-stu-id="f5761-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="f5761-106">Ja problēma joprojām pastāv, iespējams, būs jāsazinās ar tā pasta resursdatora administratoru, kuram mēģināt nosūtīt e-pasta ziņojumu.</span><span class="sxs-lookup"><span data-stu-id="f5761-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="f5761-107">Atzīmējiet detalizētu ārējo kļūdu, kas pieejama Atlekšanas ziņojumā.</span><span class="sxs-lookup"><span data-stu-id="f5761-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="f5761-108">Microsoft atbalsts, iespējams, nevarēs palīdzēt.</span><span class="sxs-lookup"><span data-stu-id="f5761-108">Microsoft support may not be able to assist further.</span></span>
