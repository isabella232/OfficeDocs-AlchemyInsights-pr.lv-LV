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
ms.openlocfilehash: 276f6b2212c9d85df726cb46a46dee7828b34c89
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/25/2019
ms.locfileid: "36545179"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="b7b5f-102">Problēmas ar MFA</span><span class="sxs-lookup"><span data-stu-id="b7b5f-102">Issues with MFA</span></span>
<span data-ttu-id="b7b5f-103">Ir dažas lietas, kas jāpārbauda, ja lietotāji nevar pieteikties, izmantojot vairāku faktoru autentifikāciju (MFA)</span><span class="sxs-lookup"><span data-stu-id="b7b5f-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="b7b5f-104">Ietekmēto lietotāju var bloķēt Azure Active Directory portālā.</span><span class="sxs-lookup"><span data-stu-id="b7b5f-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="b7b5f-105">Šādā gadījumā automātiski tiek liegta autentifikācijas mēģinājumi šim konkrētam lietotājam.</span><span class="sxs-lookup"><span data-stu-id="b7b5f-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="b7b5f-106">Lūdzu, veiciet šajā rakstā aprakstītās darbības, lai atbloķētu tos.</span><span class="sxs-lookup"><span data-stu-id="b7b5f-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="b7b5f-107">Ja atbloķēšanas lietotāja nepalīdzēja vai lietotājs nav bloķēts varat mēģināt atiestatīt MFA par lietotāju, un viņi iet caur reģistrēšanas procesu vēlreiz.</span><span class="sxs-lookup"><span data-stu-id="b7b5f-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="b7b5f-108">Lūdzu, veiciet šajā rakstā aprakstītās darbības.</span><span class="sxs-lookup"><span data-stu-id="b7b5f-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="b7b5f-109">Ja šī ir pirmā reize, kad iespējojat MFA un lietotāji nevar pieteikties-pārlūkprogrammas klientiem, piemēram, Outlook, Skype utt, varbūt ADAL (Active Directory autentifikācijas bibliotēka) nav iespējots O365 abonements.</span><span class="sxs-lookup"><span data-stu-id="b7b5f-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="b7b5f-110">Šajā gadījumā jums būs nepieciešams, lai izveidotu savienojumu ar Exchange Online PowerShell un palaist šo cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*</span><span class="sxs-lookup"><span data-stu-id="b7b5f-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>