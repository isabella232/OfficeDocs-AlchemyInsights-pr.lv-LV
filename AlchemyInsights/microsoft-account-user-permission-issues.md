---
title: Novērst problēmu - lietotājs nav atrodams directory
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 0909edc581c811fdc4683b004e0df0adbac88d1c
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/26/2019
ms.locfileid: "35249920"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="bd69a-102">Novērst problēmu - lietotājs nav atrodams directory</span><span class="sxs-lookup"><span data-stu-id="bd69a-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="bd69a-103">Ja lietotāji saņem kļūdas ziņojumu "nevar atrast lietotāju" direktorijā.</span><span class="sxs-lookup"><span data-stu-id="bd69a-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="bd69a-104">Lūdzu, mēģiniet vēlreiz kur jautājuma tipu nav lietotāja direktorijā.</span><span class="sxs-lookup"><span data-stu-id="bd69a-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="bd69a-105">Šādas darbības var pabeigt risināt problēmu.</span><span class="sxs-lookup"><span data-stu-id="bd69a-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="bd69a-106">Nodrošina to pašu kontu, kas tiek izmantots, lai pieteiktos vēlāk konta e-pasta uzaicinājumu pieņēma.</span><span class="sxs-lookup"><span data-stu-id="bd69a-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="bd69a-107">Pārliecinieties, vai lietotājs izmanto vienu un to pašu kontu uzaicināt pieņemt un pierakstīties vietnē.</span><span class="sxs-lookup"><span data-stu-id="bd69a-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="bd69a-108">Lai iegūtu vairāk informācijas, skatīt [kā pārvaldīt jūsu Microsoft kontu aizstājvārdi</a> pārvaldīt Office 365 pieteikšanās](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="bd69a-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="bd69a-109">Atrodiet katru vieta (-as), kurā lietotājs saņem kļūdas.</span><span class="sxs-lookup"><span data-stu-id="bd69a-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="bd69a-110">Pievienot "/ _layouts/15/people.aspx/membershipgroupid=0" (pēc dubultās pēdiņas) vietnes URL beigās.</span><span class="sxs-lookup"><span data-stu-id="bd69a-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="bd69a-111">Piemērs: https://_lT _"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="bd69a-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="bd69a-112">Sarakstā atlasiet lietotāju.</span><span class="sxs-lookup"><span data-stu-id="bd69a-112">Select the user from the list.</span></span>

- <span data-ttu-id="bd69a-113">Noklikšķiniet uz **Noņemt lietotāju atļaujas** no lentes.</span><span class="sxs-lookup"><span data-stu-id="bd69a-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="bd69a-114">Pievienot atpakaļ lietotājam un atkārtoti uzaicināt lietotāju.</span><span class="sxs-lookup"><span data-stu-id="bd69a-114">Add back the User and Resend the invite to the user.</span></span>

