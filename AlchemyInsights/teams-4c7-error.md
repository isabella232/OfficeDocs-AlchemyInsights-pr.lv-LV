---
title: Teams 4c7 kļūda
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700210"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="fc5fe-102">4c7 kļūda pakalpojumā Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="fc5fe-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="fc5fe-103">Šī kļūda rodas tādēļ, ka programmai Microsoft Teams ir nepieciešama veidlapu autentifikācija.</span><span class="sxs-lookup"><span data-stu-id="fc5fe-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="fc5fe-104">Kad izvietojat Active Directory Federācijas pakalpojumu (AD FS), pēc noklusējuma iekštīklam nav iespējota veidlapu autentifikācija.</span><span class="sxs-lookup"><span data-stu-id="fc5fe-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="fc5fe-105">Ja Windows integrētā autentifikācija rodas nesekmīga, saņemsit aicinājumu pierakstīties, izmantojot veidlapu autentifikāciju.</span><span class="sxs-lookup"><span data-stu-id="fc5fe-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="fc5fe-106">Lai atrisinātu šo problēmu, iespējojiet veidlapu autentifikāciju, izmantojot AD FS Microsoft pārvaldības konsoles (MMC) papildprogramma datorā, kurā ir lokālā Active Directory kopija.</span><span class="sxs-lookup"><span data-stu-id="fc5fe-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="fc5fe-107">Lai to izdarītu, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="fc5fe-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="fc5fe-108">Navigācijas rūtī pārlūkojiet līdz **autentificēšanas politikas**.</span><span class="sxs-lookup"><span data-stu-id="fc5fe-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="fc5fe-109">Detalizētās informācijas rūts sadaļā **darbības** atlasiet **Rediģēt globālo primāro autentifikāciju**.</span><span class="sxs-lookup"><span data-stu-id="fc5fe-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="fc5fe-110">Cilnē **iekštīkls** atlasiet **veidlapu autentifikācija**.</span><span class="sxs-lookup"><span data-stu-id="fc5fe-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="fc5fe-111">Atlasiet **Labi** (vai **lietot**).</span><span class="sxs-lookup"><span data-stu-id="fc5fe-111">Select **OK** (or **Apply**).</span></span>