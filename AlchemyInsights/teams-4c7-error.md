---
title: Teams 4C 7 kļūda
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796232"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="75748-102">4C 7 kļūda Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="75748-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="75748-103">Šī kļūda rodas tāpēc, ka Microsoft Teams nepieciešama veidlapu autentifikācija.</span><span class="sxs-lookup"><span data-stu-id="75748-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="75748-104">Ieviešot Active Directory Federācijas pakalpojums (AD FS), veidlapu autentifikācija nav iekštīkla pēc noklusējuma nav iespējots.</span><span class="sxs-lookup"><span data-stu-id="75748-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="75748-105">Ja Windows integrētā autentifikācija neizdodas, tiek piedāvāts pierakstīties, izmantojot veidlapu autentifikācija.</span><span class="sxs-lookup"><span data-stu-id="75748-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="75748-106">Lai novērstu šo problēmu, iespējojiet veidlapu autentifikācija, izmantojot AD FS Microsoft pārvaldības konsoles (MMC) papildprogrammu datorā, kurā ir Active Directory lokālo kopiju.</span><span class="sxs-lookup"><span data-stu-id="75748-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="75748-107">Lai to izdarītu, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="75748-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="75748-108">Navigācijas rūtī atrodiet **autentifikācijas politikas**.</span><span class="sxs-lookup"><span data-stu-id="75748-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="75748-109">Detalizētās informācijas rūts sadaļā **darbības** atlasiet **Rediģēt globālo primāro autentifikāciju**.</span><span class="sxs-lookup"><span data-stu-id="75748-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="75748-110">Cilnē **iekštīkla** atlasiet **veidlapu autentifikācija**.</span><span class="sxs-lookup"><span data-stu-id="75748-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="75748-111">Atlasiet **Labi** (vai **lietot**).</span><span class="sxs-lookup"><span data-stu-id="75748-111">Select **OK** (or **Apply**).</span></span>