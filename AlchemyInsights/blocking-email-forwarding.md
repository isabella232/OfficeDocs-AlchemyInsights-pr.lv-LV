---
title: 726 E-pasta pārsūtīšanas bloķēšana
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
ms.openlocfilehash: 0bff7ede02809e133dc6616452ec840f552bd4fa6c45b7987d6455b2a9ba49bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059639"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>E-pasta pārsūtīšanas bloķēšana vai atbloķēšana

Lai iespējotu vai atspējotu e-pasta pārsūtīšanu konkrētai pastkastei, skatiet rakstu [E-pasta pārsūtīšanas konfigurēšana.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

Nomnieka līmenī ārējās pārsūtīšanas kontrole tiek veikta, izmantojot izejošo surogātpasta politiku. Varat šeit skatīt izejošo surogātpasta filtra politiku [](https://protection.office.com/antispam) drošības un atbilstības centrā vai izmantojot komandu [Get-HostedOutboundSpamFilterPolicy.](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy)

Ja tiek parādīts šāds kļūdas ziņojums: **"550 5.7.520** Piekļuve liegta, jūsu organizācija neļauj veikt ārējo pārsūtīšanu", lūdzu, pārliecinieties, vai politika ir konfigurēta, lai iespējotu ārējo automātisko pārsūtīšanu.

**Piezīme.** Ārējo automātisko pārsūtīšanu ir ieteicams atspējot noklusējuma izejošā surogātpasta filtra politikā un iespējot to tikai tiem lietotājiem, kuriem ir nepieciešama ārējā pārsūtīšana, izveidojot šiem lietotājiem pielāgotu politiku. Papildinformāciju varat lasīt [šeit: Ārējo e-pasta ziņojumu pārsūtīšanas konfigurēšana programmā Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)