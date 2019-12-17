---
title: Novērst problēmu-lietotājs nav atrasts direktorijā
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 0f1e427801107109e31486a4d300f53084880caf
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054817"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="bff01-102">Novērst problēmu-lietotājs nav atrasts direktorijā</span><span class="sxs-lookup"><span data-stu-id="bff01-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="bff01-103">Ja lietotāji saņem kļūdas ziņojumu "lietotājs nevar atrast" direktorijā, lūdzu, mēģiniet vēlreiz, ja problēmas tips ir lietotāja nav direktorijā.</span><span class="sxs-lookup"><span data-stu-id="bff01-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="bff01-104">Šīs darbības var izpildīt, lai novērstu šo problēmu.</span><span class="sxs-lookup"><span data-stu-id="bff01-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="bff01-105">Pārliecinieties, vai konts, kas akceptējis e-pasta uzaicinājumu, ir tas pats konts, kas tiek izmantots, lai pierakstītos vēlāk.</span><span class="sxs-lookup"><span data-stu-id="bff01-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="bff01-106">Pārliecinieties, vai lietotājs izmanto to pašu kontu, lai akceptētu uzaicinājumu un pierakstītos vietnē.</span><span class="sxs-lookup"><span data-stu-id="bff01-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="bff01-107">Papildinformāciju skatiet rakstā [kā pārvaldīt Microsoft konta</a> aizstājvārdus, lai pārvaldītu Office 365 pieteikšanos](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="bff01-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="bff01-108">Atrodiet katru vietu (-as), kurā lietotājs saņem kļūdu.</span><span class="sxs-lookup"><span data-stu-id="bff01-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="bff01-109">Pievienot "/_layouts/15/People.aspx/membershipgroupid = 0" (dubultā pēdiņas) beigās vietnes URL.</span><span class="sxs-lookup"><span data-stu-id="bff01-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="bff01-110">Piemērs: https://< "Contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="bff01-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="bff01-111">Sarakstā atlasiet lietotāju.</span><span class="sxs-lookup"><span data-stu-id="bff01-111">Select the user from the list.</span></span>

- <span data-ttu-id="bff01-112">Lentē noklikšķiniet uz **Noņemt lietotāja atļaujas** .</span><span class="sxs-lookup"><span data-stu-id="bff01-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="bff01-113">Pievienojiet lietotāju atpakaļ un atkārtoti nosūtiet uzaicinājumu lietotājam.</span><span class="sxs-lookup"><span data-stu-id="bff01-113">Add back the User and Resend the invite to the user.</span></span>

