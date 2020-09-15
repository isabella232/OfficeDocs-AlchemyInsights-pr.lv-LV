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
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>E-pasta piegādes problēmu (kļūdas kods 5.7.23) novēršana

Pārbaudiet sava domēna SPF DNS ierakstu par publiski pieejamu SPF vai DNS ierakstu pārbaudītāju tīmeklī.

Pārliecinieties, ka korporācija Microsoft nav identificējusi izejošo ziņojumu kā surogātpastu un maršrutēja [lielu riska piegādes pūlu](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). Ziņojumi augsta riska piegādes pūlā neveic SPF pārbaudes, tāpēc galamērķa e-pasta organizācija nepieņems.

Ja problēma joprojām pastāv, iespējams, būs jāsazinās ar tā pasta resursdatora administratoru, kuram mēģināt nosūtīt e-pasta ziņojumu. Atzīmējiet detalizētu ārējo kļūdu, kas pieejama Atlekšanas ziņojumā. Microsoft atbalsts, iespējams, nevarēs palīdzēt.
