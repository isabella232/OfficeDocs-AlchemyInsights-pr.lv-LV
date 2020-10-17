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
ms.openlocfilehash: 2f3528375d251542fd82761d00c776706de2e23c
ms.sourcegitcommit: f7b82f75a5400e992ecbd48a666783354e2e2871
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/15/2020
ms.locfileid: "48473108"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="6dd8e-102">E-pasta pārsūtīšanas bloķēšana un atbloķēšana</span><span class="sxs-lookup"><span data-stu-id="6dd8e-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="6dd8e-103">Lai iespējotu vai atspējotu e-pasta pārsūtīšanu konkrētai pastkastei, skatiet rakstu [e-pasta pārsūtīšanas konfigurēšana](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="6dd8e-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="6dd8e-104">Nomnieka līmenī ārējo pāradresēšanas kontrole ir veikta, izmantojot izejošās surogātpasta politiku.</span><span class="sxs-lookup"><span data-stu-id="6dd8e-104">On the tenant level, control of external forwarding is done using the outbound spam policy.</span></span> <span data-ttu-id="6dd8e-105">Varat pārbaudīt izejošās surogātpasta filtrēšanas politiku no drošības un atbilstības centra [šeit] ( https://protection.office.com/antispam) vai izmantojot [komandu Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span><span class="sxs-lookup"><span data-stu-id="6dd8e-105">You can check the outbound spam filter policy from Security and Compliance Center [here] (https://protection.office.com/antispam) or by using the [Get-HostedOutboundSpamFilterPolicy command](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span></span>

<span data-ttu-id="6dd8e-106">Ja tiek parādīts šāds kļūdas ziņojums: **"550 5.7.520 piekļuve liegta, jūsu organizācija nenodrošina ārējo pārsūtīšanu"**, lūdzu, pārliecinieties, vai politika ir konfigurēta tā, lai iespējotu ārējo automātisko pāradresēšanu.</span><span class="sxs-lookup"><span data-stu-id="6dd8e-106">If you are getting the following error: **“550 5.7.520 Access denied, Your organization does not allow external forwarding”**, please make sure the policy is configured to enable External Auto-forward.</span></span>

<span data-ttu-id="6dd8e-107">**Piezīme:** Ieteicams saglabāt ārēju automātisko pārsūtīšanu atspējotu savā noklusējuma izejošās surogātpasta filtrēšanas politikā un iespējot to tikai tiem lietotājiem, kuriem ir jāveic ārēja pārsūtīšana, izveidojot pielāgotu politiku šiem lietotājiem.</span><span class="sxs-lookup"><span data-stu-id="6dd8e-107">**Note:** It is recommended to keep the External Autoforward disabled on your default outbound spam filter policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="6dd8e-108">Varat lasīt vairāk, [konfigurējot ārējo e-pasta pārsūtīšanu pakalpojumā Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="6dd8e-108">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>