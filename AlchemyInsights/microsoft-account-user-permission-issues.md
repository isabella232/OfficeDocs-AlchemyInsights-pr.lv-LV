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
ms.openlocfilehash: 537b27d06acd17cbb3fe99bcb89e153099e92bb4
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/22/2019
ms.locfileid: "36544870"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="4a4d9-102">Novērst problēmu - lietotājs nav atrodams directory</span><span class="sxs-lookup"><span data-stu-id="4a4d9-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="4a4d9-103">Ja lietotāji saņem kļūdas ziņojumu "nevar atrast lietotāju" direktorijā.</span><span class="sxs-lookup"><span data-stu-id="4a4d9-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="4a4d9-104">Lūdzu, mēģiniet vēlreiz kur jautājuma tipu nav lietotāja direktorijā.</span><span class="sxs-lookup"><span data-stu-id="4a4d9-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="4a4d9-105">Šādas darbības var pabeigt risināt problēmu.</span><span class="sxs-lookup"><span data-stu-id="4a4d9-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="4a4d9-106">Nodrošina to pašu kontu, kas tiek izmantots, lai pieteiktos vēlāk konta e-pasta uzaicinājumu pieņēma.</span><span class="sxs-lookup"><span data-stu-id="4a4d9-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="4a4d9-107">Pārliecinieties, vai lietotājs izmanto vienu un to pašu kontu uzaicināt pieņemt un pierakstīties vietnē.</span><span class="sxs-lookup"><span data-stu-id="4a4d9-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="4a4d9-108">Lai iegūtu vairāk informācijas, skatīt [kā pārvaldīt jūsu Microsoft kontu aizstājvārdi</a> pārvaldīt Office 365 pieteikšanās](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="4a4d9-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="4a4d9-109">Atrodiet katru vieta (-as), kurā lietotājs saņem kļūdas.</span><span class="sxs-lookup"><span data-stu-id="4a4d9-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="4a4d9-110">Pievienot "/ _layouts/15/people.aspx/membershipgroupid=0" (pēc dubultās pēdiņas) vietnes URL beigās.</span><span class="sxs-lookup"><span data-stu-id="4a4d9-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="4a4d9-111">Piemērs: https://_lT _"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="4a4d9-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="4a4d9-112">Sarakstā atlasiet lietotāju.</span><span class="sxs-lookup"><span data-stu-id="4a4d9-112">Select the user from the list.</span></span>

- <span data-ttu-id="4a4d9-113">Noklikšķiniet uz **Noņemt lietotāju atļaujas** no lentes.</span><span class="sxs-lookup"><span data-stu-id="4a4d9-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="4a4d9-114">Pievienot atpakaļ lietotājam un atkārtoti uzaicināt lietotāju.</span><span class="sxs-lookup"><span data-stu-id="4a4d9-114">Add back the User and Resend the invite to the user.</span></span>

