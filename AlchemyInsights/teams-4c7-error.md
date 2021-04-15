---
title: Teams 4c7 kļūda
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786676"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="d9bc9-102">Kļūda 4c7 lietojumprogrammā Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="d9bc9-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="d9bc9-103">Šī kļūda rodas tāpēc, ka Microsoft Teams pieprasa veidlapu autentifikāciju.</span><span class="sxs-lookup"><span data-stu-id="d9bc9-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="d9bc9-104">Kad izvietojat Active Directory federācijas pakalpojumu (AD FS), veidlapu autentifikācija pēc noklusējuma nav iespējota iekštīklam.</span><span class="sxs-lookup"><span data-stu-id="d9bc9-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="d9bc9-105">Ja Windows integrētā autentifikācija neizdodas, jums tiek piedāvāts pierakstīties, izmantojot veidlapu autentifikāciju.</span><span class="sxs-lookup"><span data-stu-id="d9bc9-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="d9bc9-106">Lai novērstu šo problēmu, iespējojiet Forms Authentication, izmantojot AD FS Microsoft Management Console (MMC) papildprogrammu datorā, kurā ir lokālā Active Directory kopija.</span><span class="sxs-lookup"><span data-stu-id="d9bc9-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="d9bc9-107">Lai to izdarītu, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="d9bc9-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="d9bc9-108">Navigācijas rūtī pārlūkojiet līdz **Autentifikācijas politikas**.</span><span class="sxs-lookup"><span data-stu-id="d9bc9-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="d9bc9-109">Sadaļas Darbības detalizētas informācijas rūtī atlasiet **Rediģēt globālo primāro autentifikāciju**. </span><span class="sxs-lookup"><span data-stu-id="d9bc9-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="d9bc9-110">Cilnē **Iekštīkls** atlasiet Forms **Authentication**.</span><span class="sxs-lookup"><span data-stu-id="d9bc9-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="d9bc9-111">Atlasiet **Labi** (vai **Lietot**).</span><span class="sxs-lookup"><span data-stu-id="d9bc9-111">Select **OK** (or **Apply**).</span></span>