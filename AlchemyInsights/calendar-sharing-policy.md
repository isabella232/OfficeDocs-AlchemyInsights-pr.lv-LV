---
title: 618 kalendāra koplietošanas politika
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
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684237"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Politikas kļūda, kopīgojot kalendāru

1. Atbilstoši situācijai veiciet kādu no šīm darbībām:
    - Savienojuma izveide ar Exchange Online, izmantojot Remote PowerShell. Papildinformāciju skatiet rakstā Savienojuma izveide [ar Exchange Online, izmantojot Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Lokālajā serverī atveriet Exchange pārvaldības čaulu.
2. Noteikt lietotājam piešķirto koplietošanas politiku. Lai to paveiktu, izpildiet šādu komandu un ievērojiet, ka tiek atgriezta politika:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Atjauniniet lietotāja kopīgošanas politiku. Lai to izdarītu, veiciet tālāk norādītās darbības.
    - Atveriet Exchange administrēšanas centru.
    - Noklikšķiniet uz **organizācija**un pēc tam veiciet dubultklikšķi uz lietotāja piešķirtās **politikas.** Šī ir politika, kas tika atgriezta 2. darbībā.
    - Lapā koplietošanas kārtula atlasiet kalendāra koplietošanas līmeni, kuru vēlaties atļaut sadaļā **Norādiet, kādu informāciju vēlaties koplietot**. noklikšķiniet uz **Saglabāt**.

Lai iegūtu papildinformāciju, skatiet rakstu: ["politika neļauj piešķirt atļaujas šajā līmenī vienam vai vairākiem adresātiem", ja lietotājs mēģina kopīgot kalendāru](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
