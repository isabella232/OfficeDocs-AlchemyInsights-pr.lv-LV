---
title: Problēmas ar MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755138"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="922ad-102">Problēmas ar Azure MFA</span><span class="sxs-lookup"><span data-stu-id="922ad-102">Issues with Azure MFA</span></span>
<span data-ttu-id="922ad-103">Ir daži ieteikumi, kā pārbaudīt, vai lietotāji nevar pieteikties, izmantojot daudzfaktoru autentifikāciju (MFA)</span><span class="sxs-lookup"><span data-stu-id="922ad-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="922ad-104">Ietekmētais lietotājs var tikt bloķēts Azure Active Directory portālā.</span><span class="sxs-lookup"><span data-stu-id="922ad-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="922ad-105">Ja tā ir, šī konkrētā lietotāja autentifikācijas mēģinājumi tiks automātiski noraidīti.</span><span class="sxs-lookup"><span data-stu-id="922ad-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="922ad-106">Lūdzu, veiciet šajā rakstā norādītās darbības, lai tās atbloķētu.</span><span class="sxs-lookup"><span data-stu-id="922ad-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="922ad-107">Ja atbloķēšanas lietotājs nepalīdzēja vai lietotājs nav bloķēts, varat mēģināt atiestatīt MFA lietotājam, un tie tiks pārskaitīti no jauna reģistrēšanās procesam.</span><span class="sxs-lookup"><span data-stu-id="922ad-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="922ad-108">Lūdzu, veiciet šajā rakstā norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="922ad-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="922ad-109">Ja šī ir pirmā reize, kad iespējojat MFA, un jūsu lietotāji nevar pieteikties pārlūkprogrammās, kas nav pārlūkprogrammu klienti, piemēram, Outlook, Skype utt., iespējams, ADAL (Active Directory Authentication Library) nav iespējots jūsu O365 abonementā.</span><span class="sxs-lookup"><span data-stu-id="922ad-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="922ad-110">Šajā gadījumā vajadzēs izveidot savienojumu ar Exchange Online PowerShell un palaist šo cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*</span><span class="sxs-lookup"><span data-stu-id="922ad-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>