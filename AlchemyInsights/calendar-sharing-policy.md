---
title: 618 Kalendāra koplietošanas politika
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: 1f1bfb0273301c05f5fe5f8af5fb9039328390d16305e33897680dce1c1977e8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091610"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Politikas kļūda, kopīgojot kalendāru

1. Veiciet kādu no šīm darbībām atbilstoši jūsu situācijai:
    - Savienošana, Exchange Online, izmantojot Remote PowerShell. Papildinformāciju skatiet rakstā [Savienošana, kā Exchange Online izmantot Remote PowerShell.](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)
    - Lokālajā serverī atveriet pārvaldības čaulu Exchange čaulu.
2. Nosakiet lietotājam piešķirto koplietošanas politiku. Lai to izdarītu, izpildiet šādu komandu un atzīmējiet atgriezto politiku:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Atjauniniet lietotāja koplietošanas politiku. Lai to izdarītu, veiciet tālāk norādītās darbības.
    - Atveriet Exchange administrēšanas centru.
    - Noklikšķiniet **uz** Organizācija un pēc tam veiciet dubultklikšķi uz politikas, kas lietotājam ir piešķirta sadaļā **Atsevišķa koplietošana.** Šī ir politika, kas tika atgriezta 2. darbībā.
    - Lapas Koplietošanas kārtula sadaļā Norādiet, kādu informāciju vēlaties kopīgot atlasiet kalendāra koplietošanas **līmeni, kuru vēlaties atļaut;** noklikšķiniet **uz Saglabāt**.

Papildinformāciju skatiet rakstā Kad lietotājs mēģina koplietot kalendāru, tiek parādīts ziņojums "Politika neatļauj piešķirt šī līmeņa atļaujas vienam vai vairākiem [adresātiem".](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)
