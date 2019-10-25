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
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682206"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Novērst e-pasta piegādes problēmas kļūdas kods 5.7.23

Pārbaudiet, vai jūsu domēnam ir SPF DNS ieraksts tīmeklī publiski pieejamā SPF vai DNS ierakstu pārbaudītājā.

Pārbaudiet, vai izejošais ziņojums netika identificēts kā surogātpasts Office 365 un maršrutēts, izmantojot [augsta riska piegādes pūlā](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages). Augsta riska piegādes pūla ziņojumi netiks iet SPF pārbaudes, un tādēļ netiks akceptēts mērķa e-pasta organizācijas.

Ja problēma joprojām pastāv, iespējams, vajadzēs sazināties ar administratora pasta resursdatora, kuru mēģināt nosūtīt e-pastu. Pierakstiet detalizētu ārējo kļūdu, kas pieejama ziņojumā par atlēcienu.  Office 365 atbalsts, iespējams, nevarēs palīdzēt tālāk.