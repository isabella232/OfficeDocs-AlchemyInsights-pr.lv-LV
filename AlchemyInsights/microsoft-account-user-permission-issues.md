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
ms.openlocfilehash: 81b9dafe8e27e5f73fe232c51ff56fed3fec29b4
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/04/2019
ms.locfileid: "36754199"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="49125-102">Novērst problēmu-lietotājs nav atrasts direktorijā</span><span class="sxs-lookup"><span data-stu-id="49125-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="49125-103">Ja lietotāji saņem kļūdas ziņojumu "lietotājs nevar atrast" direktorijā.</span><span class="sxs-lookup"><span data-stu-id="49125-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="49125-104">Lūdzu, mēģiniet vēlreiz, ja problēmas tips ir lietotājs nav direktorijā.</span><span class="sxs-lookup"><span data-stu-id="49125-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="49125-105">Šīs darbības var izpildīt, lai novērstu šo problēmu.</span><span class="sxs-lookup"><span data-stu-id="49125-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="49125-106">Pārliecinieties, vai konts, kas akceptējis e-pasta uzaicinājumu, ir tas pats konts, kas tiek izmantots, lai pierakstītos vēlāk.</span><span class="sxs-lookup"><span data-stu-id="49125-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="49125-107">Pārliecinieties, vai lietotājs izmanto to pašu kontu, lai akceptētu uzaicinājumu un pierakstītos vietnē.</span><span class="sxs-lookup"><span data-stu-id="49125-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="49125-108">Papildinformāciju skatiet rakstā [kā pārvaldīt Microsoft konta</a> aizstājvārdus, lai pārvaldītu Office 365 pieteikšanos](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="49125-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="49125-109">Atrodiet katru vietu (-as), kurā lietotājs saņem kļūdu.</span><span class="sxs-lookup"><span data-stu-id="49125-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="49125-110">Pievienot "/_ layouts/15/People.aspx/membershipgroupid = 0" (dubultā pēdiņas) beigās vietnes vietrādi URL.</span><span class="sxs-lookup"><span data-stu-id="49125-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="49125-111">Piemērs: https://< "contoso">. SharePoint. com/_layouts/15/People. aspx/membershipGroupId = 0.</span><span class="sxs-lookup"><span data-stu-id="49125-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="49125-112">Sarakstā atlasiet lietotāju.</span><span class="sxs-lookup"><span data-stu-id="49125-112">Select the user from the list.</span></span>

- <span data-ttu-id="49125-113">Lentē noklikšķiniet uz **Noņemt lietotāja atļaujas** .</span><span class="sxs-lookup"><span data-stu-id="49125-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="49125-114">Pievienojiet lietotāju atpakaļ un atkārtoti nosūtiet uzaicinājumu lietotājam.</span><span class="sxs-lookup"><span data-stu-id="49125-114">Add back the User and Resend the invite to the user.</span></span>

