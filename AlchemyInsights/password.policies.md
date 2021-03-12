---
title: Paroļu politikas
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 826e266d08aa68c0d4213d8058a0244f404fe965
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744989"
---
# <a name="password-policies"></a><span data-ttu-id="a77fc-102">Paroļu politikas</span><span class="sxs-lookup"><span data-stu-id="a77fc-102">Password policies</span></span>

<span data-ttu-id="a77fc-103">**Man ir problēmas ar lietotāja paroļu politiku**</span><span class="sxs-lookup"><span data-stu-id="a77fc-103">**I'm having problems with the password policy for a user**</span></span>

- <span data-ttu-id="a77fc-104">Lietotāja paroļu politika ir atkarīga no tā, vai lietotājs ir tikai mākonī vai lokāli.</span><span class="sxs-lookup"><span data-stu-id="a77fc-104">The password policy for a user depends on whether the user is cloud only or on-premises.</span></span>
- <span data-ttu-id="a77fc-105">Tikai mākonī lietotājiem ir jāizvēlas parole, kas atbilst šī raksta prasībām: [paroļu politikas, kas attiecas tikai uz mākoņa lietotāju kontiem](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span><span class="sxs-lookup"><span data-stu-id="a77fc-105">Cloud only users must choose a password that meets the requirements in this article: [Password policies that only apply to cloud user accounts](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span></span>
- <span data-ttu-id="a77fc-106">Lokālajiem lietotājiem ir jāizvēlas parole, kas atbilst lokālajām prasībām.</span><span class="sxs-lookup"><span data-stu-id="a77fc-106">On-premises users must choose a password that meets the on-premises requirements.</span></span> <span data-ttu-id="a77fc-107">Ja lokālais lietotājs nevar iestatīt savu paroli, skatiet lokālās prasības.</span><span class="sxs-lookup"><span data-stu-id="a77fc-107">If an on-premises user is unable to set their password, check your on-premises requirements.</span></span>

<span data-ttu-id="a77fc-108">**Es nezinu, kā iestatīt vai pārbaudīt paroļu derīguma politikas**</span><span class="sxs-lookup"><span data-stu-id="a77fc-108">**I don't know how to set or check password expiration policies**</span></span>

- <span data-ttu-id="a77fc-109">Varat iestatīt un skatīt mākoņa lietotāju derīguma politiku savā nomniekā, izmantojot PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a77fc-109">You can set and check the expiration policy for cloud users in your tenant by using PowerShell.</span></span> <span data-ttu-id="a77fc-110">Izpildiet šajā rakstā sniegtos norādījumus: [iestatiet vai pārbaudiet paroļu politikas, izmantojot PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span><span class="sxs-lookup"><span data-stu-id="a77fc-110">Follow the instructions in this article: [Set or check the password policies by using PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span></span>
- <span data-ttu-id="a77fc-111">Paroļu derīguma politika lokālajiem lietotājiem tiek iestatīta jūsu lokālajā REKLĀMā.</span><span class="sxs-lookup"><span data-stu-id="a77fc-111">The password expiration policy for on-premises users is set in your on-premises AD.</span></span>

<span data-ttu-id="a77fc-112">**Citas noderīgas saites:**</span><span class="sxs-lookup"><span data-stu-id="a77fc-112">**Other Helpful links:**</span></span>
- [<span data-ttu-id="a77fc-113">Darba sākšana ar paroles atiestatīšanu</span><span class="sxs-lookup"><span data-stu-id="a77fc-113">Getting Started with Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [<span data-ttu-id="a77fc-114">Administratora iniciētas paroles atiestatīšanas problēmu novēršana</span><span class="sxs-lookup"><span data-stu-id="a77fc-114">Troubleshoot Administrator-initiated Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
