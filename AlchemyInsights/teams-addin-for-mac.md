---
title: Teams pievienojumprogramma darbam ar Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 74bd424f71a59b80a91b960b815363668bee7036
ms.sourcegitcommit: 1361b2b37fd0201502a1a3547084961de284a3fc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/11/2020
ms.locfileid: "46629687"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="58f3a-102">Teams pievienojumprogramma darbam ar Mac</span><span class="sxs-lookup"><span data-stu-id="58f3a-102">Teams add-in for Mac</span></span>

<span data-ttu-id="58f3a-103">Lai novērstu problēmas saistībā ar trūkstošo grupu pievienojumprogrammu darbam ar Mac operētājsistēmu lietotājiem, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="58f3a-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="58f3a-104">**1. darbība:** Ja jums ir hibrīda Exchange lokāli (2016 CU3 vai jaunāka versija), izmantojiet Test-HMA.ps1 rīku, lai apstiprinātu, ka hibrīdā modernā autentifikācija ir pareizi konfigurēta.</span><span class="sxs-lookup"><span data-stu-id="58f3a-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="58f3a-105">Papildinformāciju skatiet rakstā [hibrīdās modernās autentifikācijas iestatīšana programmā Outlook darbam ar iOS un Android](https://aka.ms/AA980zq).</span><span class="sxs-lookup"><span data-stu-id="58f3a-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/AA980zq).</span></span>  

<span data-ttu-id="58f3a-106">**Piezīmes** Izmantojiet UPN adreses formātu (piemēram, [username@contoso.com](mailto:username@contoso.com)), not domēns \ lietotājvārds</span><span class="sxs-lookup"><span data-stu-id="58f3a-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="58f3a-107">To var paveikt arī lietotājiem, kuriem ir Exchange Online pastkastes.</span><span class="sxs-lookup"><span data-stu-id="58f3a-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="58f3a-108">**2. darbība.** Vai lietotājam ir jāpāriet uz **rīku**  >  **konti**... programmā Outlook darbam ar Mac atrodiet un atlasiet kontu.</span><span class="sxs-lookup"><span data-stu-id="58f3a-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="58f3a-109">Apstipriniet, ka sarakstā norādītais lietotājvārds ir UPN formātā (piemēram, [username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="58f3a-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="58f3a-110">**3. darbība:** Apstipriniet, ka lietotājs ir licencēts Microsoft Teams lietotājs.</span><span class="sxs-lookup"><span data-stu-id="58f3a-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="58f3a-111">Lietotājam ir jāizmanto Office 365 for Mac abonements, produkta versija 16,24 vai jaunāka versija.</span><span class="sxs-lookup"><span data-stu-id="58f3a-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>