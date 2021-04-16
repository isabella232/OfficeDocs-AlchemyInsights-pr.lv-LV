---
title: Problēmas ar MFA
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810491"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="aeeb6-102">Problēmas ar Azure MFA</span><span class="sxs-lookup"><span data-stu-id="aeeb6-102">Issues with Azure MFA</span></span>
<span data-ttu-id="aeeb6-103">Ir dažas lietas, kas jāpārbauda, vai lietotāji nevar pieteikties, izmantojot daudz faktoru autentificēšanu (MFA)</span><span class="sxs-lookup"><span data-stu-id="aeeb6-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="aeeb6-104">Ietekmēto lietotāju var bloķēt Azure Active Directory portālā.</span><span class="sxs-lookup"><span data-stu-id="aeeb6-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="aeeb6-105">Šādā gadījumā konkrētam lietotājam autentifikācijas mēģinājumi tiks automātiski noraidīti.</span><span class="sxs-lookup"><span data-stu-id="aeeb6-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="aeeb6-106">Izpildiet šajā rakstā minētās darbības, lai tās atbloķētu.</span><span class="sxs-lookup"><span data-stu-id="aeeb6-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="aeeb6-107">Ja lietotāja atbloķēšana nepalīdzēja vai lietotājs nav bloķēts, varat mēģināt atiestatīt lietotāja MFA un viņš vēlreiz veiks reģistrācijas procesu.</span><span class="sxs-lookup"><span data-stu-id="aeeb6-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="aeeb6-108">Izpildiet šajā rakstā norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="aeeb6-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="aeeb6-109">Ja šī ir pirmā reize, kad iespējojat MFA un jūsu lietotāji nevar pieteikties klientiem, kas nav pārlūkprogrammas, piemēram, Outlook, Skype un citiem, iespējams, ADAL (Active Directory Authentication Library — Active Directory autentifikācijas bibliotēka) jūsu O365 abonementā nav iespējota.</span><span class="sxs-lookup"><span data-stu-id="aeeb6-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="aeeb6-110">Šajā gadījumā būs jāizveido savienojums ar Exchange Online Powershell un jāpalaiž šis cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span><span class="sxs-lookup"><span data-stu-id="aeeb6-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>