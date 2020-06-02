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
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Novērst e-pasta piegādes problēmas kļūdas kods 5.7.23

Pārbaudiet, vai jūsu domēnam ir SPF DNS ieraksts tīmeklī publiski pieejamā SPF vai DNS ierakstu pārbaudītājā.

Pārbaudiet, vai izejošais ziņojums netika identificēts kā Microsoft surogātpasts un maršrutēts, izmantojot [augsta riska piegādes pūlu](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). Augsta riska piegādes pūla ziņojumi netiks iet SPF pārbaudes, un tādēļ netiks akceptēts mērķa e-pasta organizācijas.

Ja problēma joprojām pastāv, iespējams, vajadzēs sazināties ar administratora pasta resursdatora, kuru mēģināt nosūtīt e-pastu. Pierakstiet detalizētu ārējo kļūdu, kas pieejama ziņojumā par atlēcienu. Iespējams, ka Microsoft atbalsts nevarēs palīdzēt tālāk.
