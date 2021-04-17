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
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>E-pasta piegādes problēmu (kļūdas kods 5.7.23) novēršana

Pārbaudiet sava domēna SPF DNS ierakstu publiski pieejama SPF vai DNS ieraksta pārbaudītājā tīmeklī.

Pārbaudiet, vai korporācija Microsoft nav identificējusi izejošo ziņojumu kā surogātpastu un maršrutēta, izmantojot augsta [riska piegādes pūlu.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) Ziņojumi augsta riska piegādes pūlā neiztur SPF pārbaudes, tāpēc mērķa e-pasta organizācijā tos nepieņems.

Ja problēma joprojām pastāv, iespējams, ir jāsazinās ar tā pasta viesošanas pakalpojumu resursdatora administratoru, kuram mēģināt nosūtīt e-pastu. Pievērsiet uzmanību detalizētai ārējai kļūdai, kas pieejama atlēciena ziņojumā. Iespējams, Microsoft atbalsta dienests nevarēs jums palīdzēt.
