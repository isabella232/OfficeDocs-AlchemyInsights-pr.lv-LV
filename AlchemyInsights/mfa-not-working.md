---
title: Problēmas ar MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2e79040c249b7825b964a19c51bcc42e5a6afb3f
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/26/2019
ms.locfileid: "35250172"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="006f6-102">Problēmas ar MFA</span><span class="sxs-lookup"><span data-stu-id="006f6-102">Issues with MFA</span></span>
<span data-ttu-id="006f6-103">Ir pāris lietas, lai pārbaudītu, ja lietotāji nevar reģistrēties sistēmā, izmantojot vairāku faktoru autentifikaciju (MFA)</span><span class="sxs-lookup"><span data-stu-id="006f6-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="006f6-104">Skarto lietotāju var tikt bloķēta Azure Active Directory portālā.</span><span class="sxs-lookup"><span data-stu-id="006f6-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="006f6-105">Ja tas tā ir gadījumā, autentifikācijas mēģinājumus, ka konkrētu lietotāju būs automātiski noraidīja.</span><span class="sxs-lookup"><span data-stu-id="006f6-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="006f6-106">Lūdzu izpildiet šajā pantā atbloķēt tos.</span><span class="sxs-lookup"><span data-stu-id="006f6-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="006f6-107">Ja atbloķēšanas lietotājam nepalīdzēja vai nav bloķēts lietotājs jūs varat mēģināt atiestatīt lietotāja MFA un viņi iet cauri procesam enroll atkal.</span><span class="sxs-lookup"><span data-stu-id="006f6-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="006f6-108">Lūdzu, izpildiet šajā rakstā aprakstītie soļi.</span><span class="sxs-lookup"><span data-stu-id="006f6-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="006f6-109">Ja šī ir pirmā reize, kad ļāva MFA un lietotāji nevarat ieiet bez pārlūkprogrammas klientiem, piemēram, Outlook, Skype u.c., varbūt ADAL (aktīvajā direktorijā autentifikācijas bibliotēka) nav iespējota O365 abonementu.</span><span class="sxs-lookup"><span data-stu-id="006f6-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="006f6-110">Šajā gadījumā jums būs nepieciešams pieslēgties Exchange Online Powershell un palaist šo cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="006f6-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>