---
title: SMTP autentifikācijas problēmu novēršana
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826422"
---
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="f6e51-102">SMTP autentifikācijas problēmu novēršana</span><span class="sxs-lookup"><span data-stu-id="f6e51-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="f6e51-103">Ja, mēģinot nosūtīt SMTP e-pastu un autentificēšanu klientā vai lietojumprogrammā, rodas kļūdas 5.7.57 vai 5.7.3, ir dažas lietas, kas jāpārbauda:</span><span class="sxs-lookup"><span data-stu-id="f6e51-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="f6e51-104">Autentificēts SMTP iesniegšana var būt atspējota jūsu nomniekā vai pastkastē, kuru mēģināt izmantot (pārbaudiet abus iestatījumus).</span><span class="sxs-lookup"><span data-stu-id="f6e51-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="f6e51-105">Papildinformāciju skatiet rakstā Autentificēta klienta SMTP iesniegšanas iespējošana [vai atspējošana.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)</span><span class="sxs-lookup"><span data-stu-id="f6e51-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="f6e51-106">Pārbaudiet, [vai jūsu nomniekam](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) ir iespējoti Azure drošības noklusējums. ja iespējota, SMTP autentifikācija, izmantojot pamata autentifikāciju (tiek dēvēta arī par mantoto; tas izmantos lietotājvārdu un paroli) neizdosies.</span><span class="sxs-lookup"><span data-stu-id="f6e51-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>
