---
title: 618 kalendāra koplietošanas politika
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/26/2020
ms.locfileid: "44373006"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Politikas kļūda, koplietojot kalendāru

1. Veiciet kādu no šīm darbībām atbilstoši situācijai:
    - Izveidot savienojumu ar Exchange Online, izmantojot attālo PowerShell. Lai iegūtu papildinformāciju, skatiet [izveidot savienojumu ar Exchange Online, izmantojot attālo PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Lokālas serverī atveriet Exchange pārvaldības čaulu.
2. Nosakiet koplietošanas politikas, kas ir piešķirts lietotājam. Lai to paveiktu, izpildiet šādu komandu un iegaumējiet atgriezto politiku:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Atjauniniet lietotāja koplietošanas politiku. Lai to izdarītu, veiciet tālāk norādītās darbības.
    - Atveriet Exchange administrēšanas centrs.
    - Noklikšķiniet uz **organizācija**un pēc tam veiciet dubultklikšķi uz politikas, kas ir piešķirta lietotājam sadaļā **individuāla koplietošana**. Šī ir politika, kas tika atgriezta 2. darbībā.
    - Lapā koplietošanas kārtula atlasiet kalendāra koplietošanas līmeni, kuru vēlaties atļaut sadaļā **Norādiet, kādu informāciju vēlaties kopīgot**; noklikšķiniet uz **saglabāt**.

Lai iegūtu papildinformāciju, skatiet: ["politika neatļauj šajā līmenī piešķirt atļaujas vienam vai vairākiem adresātiem" kļūda, kad lietotājs mēģina koplietot kalendāru](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
