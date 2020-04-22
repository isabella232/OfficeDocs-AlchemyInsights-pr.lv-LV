---
title: 1048 5.7.750 pakalpojums nav pieejams. Klients ir bloķējis sūtīšanu no nereģistrētiem domēniem
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 48b9c2de27f8d7f52215c3a3d547bdf746a3a4cd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676720"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="ec727-103">5.7.750 klients ir bloķēts no nosūtīšanas no nereģistrēta domēna</span><span class="sxs-lookup"><span data-stu-id="ec727-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="ec727-104">Kļūda rodas, ja liela apjoma ziņojumi tiek sūtīti no domēniem, kas nav nodrošināta jūsu nomnieka (pievienots kā akceptēts domēnu un validēt).</span><span class="sxs-lookup"><span data-stu-id="ec727-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="ec727-105">Lai izvairītos no šīs kļūdas, var izmantot sertifikātu sistēma pasta plūsmas savienotājs, ja sertifikāta domēns ir nodrošināta domēna, vai varat nodrošināt visas sūtīšanas domēnu.</span><span class="sxs-lookup"><span data-stu-id="ec727-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
