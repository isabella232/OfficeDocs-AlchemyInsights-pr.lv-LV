---
title: 726 e-pasta pārsūtīšanas bloķēšana
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219862"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>E-pasta pārsūtīšanas bloķēšana un atbloķēšana

Lai iespējotu vai atspējotu e-pasta pārsūtīšanu konkrētai pastkastei, skatiet rakstu [e-pasta pārsūtīšanas konfigurēšana](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Nomnieka līmenī ārējo pāradresēšanas kontrole ir veikta, izmantojot izejošo pretsurogātpasta politiku. Ja tas ir iestatīts uz izslēgts vai automātiski, tas var bloķēt e-pasta pārsūtīšanu, izmantojot "550 5.7.520 Access denied, jūsu organizācija neļauj veikt ārējo pārsūtīšanu". Pēc tam, ja pārsūtīšana ir iestatīta kā bloķēta, tā ir kļūda, ko lietotāji redzēs.

Ja pārsūtīšana tiek bloķēta, lūdzu, pārliecinieties, vai politika ir konfigurēta tā, lai iespējotu ārēju pāradresēšanu. Varat pārbaudīt izejošās surogātpasta filtrēšanas politiku no drošības un atbilstības centra vai palaist komandu Get-HostedOutboundSpamFilterPolicy | FL nosaukums AutoForwardingMode. Ja vēlaties iestatīt autopārsūtīšanas bloķēšanu, tā pati komanda izstāstīs politikas stāvokli tūlīt.

Piezīme: ieteicams paturēt ārējo automātisko pārsūtīšanu atspējotu savā noklusējuma izejošās surogātpasta filtrēšanas politikā un iespējot to tikai tiem lietotājiem, kuriem ir jāveic ārēja pārsūtīšana, izveidojot pielāgotu politiku šiem lietotājiem. Varat lasīt vairāk, [konfigurējot ārējo e-pasta pārsūtīšanu pakalpojumā Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).