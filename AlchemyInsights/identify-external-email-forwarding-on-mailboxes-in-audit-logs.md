---
title: Identificēt ārējiem e-pasta pāradresācija uz pastkastēm, audita žurnālos
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 7fb2c161c558a7eb961f86ca2b86e33750d902fd
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909385"
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
