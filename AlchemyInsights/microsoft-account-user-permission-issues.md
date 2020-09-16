---
title: Problēmu novēršana — lietotājs nav atrasts direktorijā
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725414"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="70b6c-102">Problēmu novēršana — lietotājs nav atrasts direktorijā</span><span class="sxs-lookup"><span data-stu-id="70b6c-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="70b6c-103">Ja lietotāji direktorijā saņem kļūdas ziņojumu "lietotājs nav atrasts", lūdzu, mēģini vēlreiz, kur problēmas tips ir lietotājs nav direktorijā.</span><span class="sxs-lookup"><span data-stu-id="70b6c-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="70b6c-104">Lai novērstu šo problēmu, varat veikt tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="70b6c-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="70b6c-105">Pārliecinieties, vai konts, kas pieņēma e-pasta uzaicinājumu, ir tas pats konts, kas tiek izmantots, lai pierakstītos vēlāk.</span><span class="sxs-lookup"><span data-stu-id="70b6c-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="70b6c-106">Pārliecinieties, vai lietotājs izmanto to pašu kontu, lai akceptētu uzaicinājumu un pierakstītos vietnē.</span><span class="sxs-lookup"><span data-stu-id="70b6c-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="70b6c-107">Papildinformāciju skatiet rakstā [kā pārvaldīt Microsoft konta aizstājvārdus, </a> lai pārvaldītu Microsoft 365 pieteikšanos](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="70b6c-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="70b6c-108">Pārlūkojiet līdz katrai vietnei (-ām), kurā lietotājs saņem kļūdas ziņojumu.</span><span class="sxs-lookup"><span data-stu-id="70b6c-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="70b6c-109">Pievienojiet "/_layouts/15/People.aspx/membershipgroupid = 0" (Dubultajos pēdiņās) līdz vietnes vietrāža URL beigām.</span><span class="sxs-lookup"><span data-stu-id="70b6c-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="70b6c-110">Piemērs: https://< "Contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="70b6c-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="70b6c-111">Sarakstā atlasiet lietotāju.</span><span class="sxs-lookup"><span data-stu-id="70b6c-111">Select the user from the list.</span></span>

- <span data-ttu-id="70b6c-112">Lentē noklikšķiniet uz **Noņemt lietotāja atļaujas** .</span><span class="sxs-lookup"><span data-stu-id="70b6c-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="70b6c-113">Pievienojiet lietotāju atpakaļ un vēlreiz nosūtiet uzaicinājumu lietotājam.</span><span class="sxs-lookup"><span data-stu-id="70b6c-113">Add back the User and Resend the invite to the user.</span></span>

