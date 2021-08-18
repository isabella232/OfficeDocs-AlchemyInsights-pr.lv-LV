---
title: Ārējās automātiskās e-pasta pārsūtīšanas bloķēšana vai atbloķēšana
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
ms.openlocfilehash: 6c4ddd53ab794ffad3179dd86a8f81785567cfe34240dff2aa0a1df11094883d
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/11/2021
ms.locfileid: "57897475"
---
# <a name="block-or-unblock-eternal-automatic-email-forwarding"></a>Automātiskās e-pasta pārsūtīšanas bloķēšana vai atbloķēšana

Lai iespējotu vai atspējotu e-pasta pārsūtīšanu konkrētai pastkastei, skatiet rakstu [E-pasta pārsūtīšanas konfigurēšana.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

Administratori var kontrolēt organizācijas ārējo pārsūtīšanu, izmantojot [izejošo surogātpasta politiku.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy) Jūs pārvaldāt izejošo surogātpasta politikas Microsoft 365 Defender vietnē vai izmantojot <https://security.microsoft.com/antispam> [cmdlet Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy) Exchange Online PowerShell.

Ja tiek parādīts šāds kļūdas ziņojums: **"550 5.7.520** Piekļuve liegta, jūsu organizācija neļauj veikt ārējo pārsūtīšanu", pārliecinieties, vai politika ir konfigurēta, lai iespējotu ārējos automātiski pārsūtītos ziņojumus.

**Piezīme.** Mēs iesakām  noklusējuma vērtību Automātiski  — sistēma tiek kontrolēta automātiskās pārsūtīšanas kārtulu iestatījumam jūsu noklusējuma izejošā surogātpasta filtra politikā (automātiskā ārējā pārsūtīšana ir bloķēta; joprojām darbojas iekšējā automātiskā pārsūtīšana). Izveidojiet pielāgotas izejošo surogātpasta filtra politikas un izmantojiet vērtību Ieslēgts **—** pārsūtīšana ir iespējota tikai lietotājiem, kuriem nepieciešama ārējā automātiskā e-pasta pārsūtīšana. Papildinformāciju skatiet rakstā [Ārējo e-pasta pārsūtīšanas konfigurēšana programmā Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)
