---
title: Identificēt ārējiem e-pasta pāradresācija uz pastkastēm, audita žurnālos
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 518e4dd485ee7c54ce83e65794152e32f4c3a836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752010"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Noteikt, kad ir konfigurēta ārējiem e-pasta pāradresācija pastkastēm

Kad lietotājs konfigurē ārējiem e-pasta pāradresācija uz pastkasti, darbība tiek veikta revīzija, kā daļa no **Kopas-Mailbox** cmdlet. Jūs varat redzēt, izmantojot audita žurnālu meklēšana drošības & Center izpildes darbības.

1. [Office drošības 365 & atbilstību centra](https://protection.office.com/) pieteikties

2. Noklikšķiniet uz **meklēšanas un izmeklēšanas** un atlasiet **Audita žurnālu meklēšana**.

3. Atlasiet datumu diapazona **sākuma datums** un **beigu datums** laukos. Jums nav nepieciešams norādīt lietotājvārdu. Pārbaudīt **darbības** lauks ir iestatīts uz **Parādīt visas darbības rezultātus**.

4. Noklikšķiniet uz **Meklēt**.

Rezultātos, noklikšķiniet uz **Filtrēt rezultātus** un darbības filtrs lodziņā ierakstiet **Set pastkastes** . Atlasiet ierakstu audita rezultātiem. Flyout **detaļas** , noklikšķiniet uz **Papildinformācija**. Jums ir aplūkot detalizētu informāciju par katru audita ierakstu, lai noteiktu, ja darbība ir saistīta ar e-pasta pāradresācija.

- **ObjectId**: aizstājvārds vērtība pastkasti, kura tika modificēta.

- **Parametri**: _ForwardingSmtpAddress_ norāda mērķa e-pasta adresi.

- **UserId**: lietotāju, kas ir konfigurēta e-pasta pāradresāciju uz **ObjectId** laukā pastkastes.

Plašāku informāciju skatiet [noteikšana, kas izveido e-pasta pāradresācija uz pastkasti](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
