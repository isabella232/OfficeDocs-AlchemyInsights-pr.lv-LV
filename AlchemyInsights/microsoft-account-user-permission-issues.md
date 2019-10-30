---
title: Novērst problēmu-lietotājs nav atrasts direktorijā
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 59713231da25be441e7c05d788337e66bf17265a
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768808"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="12053-102">Novērst problēmu-lietotājs nav atrasts direktorijā</span><span class="sxs-lookup"><span data-stu-id="12053-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="12053-103">Ja lietotāji saņem kļūdas ziņojumu "lietotājs nevar atrast" direktorijā, lūdzu, mēģiniet vēlreiz, ja problēmas tips ir lietotāja nav direktorijā.</span><span class="sxs-lookup"><span data-stu-id="12053-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="12053-104">Šīs darbības var izpildīt, lai novērstu šo problēmu.</span><span class="sxs-lookup"><span data-stu-id="12053-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="12053-105">Pārliecinieties, vai konts, kas akceptējis e-pasta uzaicinājumu, ir tas pats konts, kas tiek izmantots, lai pierakstītos vēlāk.</span><span class="sxs-lookup"><span data-stu-id="12053-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="12053-106">Pārliecinieties, vai lietotājs izmanto to pašu kontu, lai akceptētu uzaicinājumu un pierakstītos vietnē.</span><span class="sxs-lookup"><span data-stu-id="12053-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="12053-107">Papildinformāciju skatiet rakstā [kā pārvaldīt Microsoft konta</a> aizstājvārdus, lai pārvaldītu Office 365 pieteikšanos](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="12053-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="12053-108">Atrodiet katru vietu (-as), kurā lietotājs saņem kļūdu.</span><span class="sxs-lookup"><span data-stu-id="12053-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="12053-109">Pievienot "/_layouts/15/People.aspx/membershipgroupid = 0" (dubultā pēdiņas) beigās vietnes URL.</span><span class="sxs-lookup"><span data-stu-id="12053-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="12053-110">Piemērs: https://< "Contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="12053-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="12053-111">Sarakstā atlasiet lietotāju.</span><span class="sxs-lookup"><span data-stu-id="12053-111">Select the user from the list.</span></span>

- <span data-ttu-id="12053-112">Lentē noklikšķiniet uz **Noņemt lietotāja atļaujas** .</span><span class="sxs-lookup"><span data-stu-id="12053-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="12053-113">Pievienojiet lietotāju atpakaļ un atkārtoti nosūtiet uzaicinājumu lietotājam.</span><span class="sxs-lookup"><span data-stu-id="12053-113">Add back the User and Resend the invite to the user.</span></span>

