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
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="b7674-102">E-pasta pārsūtīšanas bloķēšana un atbloķēšana</span><span class="sxs-lookup"><span data-stu-id="b7674-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="b7674-103">Lai iespējotu vai atspējotu e-pasta pārsūtīšanu konkrētai pastkastei, skatiet rakstu [e-pasta pārsūtīšanas konfigurēšana](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="b7674-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="b7674-104">Nomnieka līmenī ārējo pāradresēšanas kontrole ir veikta, izmantojot izejošo pretsurogātpasta politiku.</span><span class="sxs-lookup"><span data-stu-id="b7674-104">On the tenant level, control of External forwarding is done using the outbound anti-spam policy.</span></span> <span data-ttu-id="b7674-105">Ja tas ir iestatīts uz izslēgts vai automātiski, tas var bloķēt e-pasta pārsūtīšanu, izmantojot "550 5.7.520 Access denied, jūsu organizācija neļauj veikt ārējo pārsūtīšanu".</span><span class="sxs-lookup"><span data-stu-id="b7674-105">If it is set to Off or Automatic, it might block email forwarding with the “550 5.7.520 Access denied, Your organization does not allow external forwarding” error.</span></span> <span data-ttu-id="b7674-106">Pēc tam, ja pārsūtīšana ir iestatīta kā bloķēta, tā ir kļūda, ko lietotāji redzēs.</span><span class="sxs-lookup"><span data-stu-id="b7674-106">Subsequently, if forwarding was set to be blocked, that is the error your users will see.</span></span>

<span data-ttu-id="b7674-107">Ja pārsūtīšana tiek bloķēta, lūdzu, pārliecinieties, vai politika ir konfigurēta tā, lai iespējotu ārēju pāradresēšanu.</span><span class="sxs-lookup"><span data-stu-id="b7674-107">If forwarding is being blocked, please make sure the policy is configured to enable External Autoforward.</span></span> <span data-ttu-id="b7674-108">Varat pārbaudīt izejošās surogātpasta filtrēšanas politiku no drošības un atbilstības centra vai palaist komandu Get-HostedOutboundSpamFilterPolicy | FL nosaukums AutoForwardingMode.</span><span class="sxs-lookup"><span data-stu-id="b7674-108">You can check the Outbound Spam Filter Policy from Security and Compliance Center or by running command Get-HostedOutboundSpamFilterPolicy | fl name,AutoForwardingMode.</span></span> <span data-ttu-id="b7674-109">Ja vēlaties iestatīt autopārsūtīšanas bloķēšanu, tā pati komanda izstāstīs politikas stāvokli tūlīt.</span><span class="sxs-lookup"><span data-stu-id="b7674-109">If you want to set up Autoforward blocking, the same command will tell you the state of policy now.</span></span>

<span data-ttu-id="b7674-110">Piezīme: ieteicams paturēt ārējo automātisko pārsūtīšanu atspējotu savā noklusējuma izejošās surogātpasta filtrēšanas politikā un iespējot to tikai tiem lietotājiem, kuriem ir jāveic ārēja pārsūtīšana, izveidojot pielāgotu politiku šiem lietotājiem.</span><span class="sxs-lookup"><span data-stu-id="b7674-110">Note: It is recommended to keep the External Autoforward disabled on your Default Outbound Spam Filter Policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="b7674-111">Varat lasīt vairāk, [konfigurējot ārējo e-pasta pārsūtīšanu pakalpojumā Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="b7674-111">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>