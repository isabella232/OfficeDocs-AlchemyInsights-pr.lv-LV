---
title: Teams for Mac pievienojumprogramma
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: 45df4381688335f10f6699d8b5ff1aaafd6f7257
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/20/2021
ms.locfileid: "52582077"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="7361c-102">Teams for Mac pievienojumprogramma</span><span class="sxs-lookup"><span data-stu-id="7361c-102">Teams add-in for Mac</span></span>

<span data-ttu-id="7361c-103">Lai novērstu problēmas, Teams pievienojumprogrammas operētājsistēmai Mac lietotājiem, rīkojieties šādi:</span><span class="sxs-lookup"><span data-stu-id="7361c-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="7361c-104">**1. darbība.** Ja izmantojat hibrīdo Exchange (2016. gada 3. vai jaunāku versiju), izmantojiet Test-HMA.ps1 rīku, lai apstiprinātu, ka hibrīdā modernā autentifikācija ir pareizi konfigurēta.</span><span class="sxs-lookup"><span data-stu-id="7361c-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="7361c-105">Papildinformāciju skatiet rakstā [Hibrīdās modernās autentifikācijas iestatīšanas validēšana Outlook iOS un Android ierīcēm.](https://aka.ms/TestHMAEAS)</span><span class="sxs-lookup"><span data-stu-id="7361c-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/TestHMAEAS).</span></span>  

<span data-ttu-id="7361c-106">**Piezīme** Izmantojiet UPN adreses formātu (piemēram, [username@contoso.com](mailto:username@contoso.com)), nevis domēns\lietotājvārds.</span><span class="sxs-lookup"><span data-stu-id="7361c-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="7361c-107">Tas ir iespējams pat lietotājiem ar Exchange Online pastkastēm.</span><span class="sxs-lookup"><span data-stu-id="7361c-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="7361c-108">**2. darbība.** Lai lietotājs pārietu uz rīku   >  **kontiem...** programmā Outlook for Mac, atrodiet un atlasiet kontu.</span><span class="sxs-lookup"><span data-stu-id="7361c-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="7361c-109">Apstipriniet lietotājvārdu, kas norādīts UPN formātā (piemēram, [username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="7361c-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="7361c-110">**3. darbība.** Pārliecinieties, vai lietotājs ir licencēts Microsoft Teams lietotājs.</span><span class="sxs-lookup"><span data-stu-id="7361c-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="7361c-111">Lietotājam jāizmanto operētājsistēmas Mac Office 365 versija 16.24 vai jaunāka versija.</span><span class="sxs-lookup"><span data-stu-id="7361c-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>