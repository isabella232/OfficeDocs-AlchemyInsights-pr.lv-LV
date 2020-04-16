---
title: Automātisko atbilžu iestatīšana pastkastē
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: aeeb2e1e76fe602d2767b422797452fd1155fdd5
ms.sourcegitcommit: fdfd41c2bfb2d45003b3906e6469377384a91cb5
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2020
ms.locfileid: "43509508"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="38677-102">Automātisko atbilžu iestatīšana lietotāja pastkastē</span><span class="sxs-lookup"><span data-stu-id="38677-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="38677-103">**1. metode**</span><span class="sxs-lookup"><span data-stu-id="38677-103">**Method 1**</span></span>

1. <span data-ttu-id="38677-104">Pierakstieties Office 365 portālā.</span><span class="sxs-lookup"><span data-stu-id="38677-104">Sign in to the Office 365 portal.</span></span>

2. <span data-ttu-id="38677-105">Dodieties uz **Lietotāji > Aktīvie lietotāji** (vai **Grupas > Koplietojamās pastkastes**, ja esat iestatījis šo kā koplietojamo pastkasti).</span><span class="sxs-lookup"><span data-stu-id="38677-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="38677-106">Atlasiet lietotāju, kuram ir Microsoft Exchange pastkaste.</span><span class="sxs-lookup"><span data-stu-id="38677-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="38677-107">Uznirstošajā izvēlnē labajā pusē dodieties uz **Pasta iestatījumi > Automātiskās atbildes** (ja tā ir koplietojama pastkaste, vienkārši izvēlnē noklikšķiniet uz **Automātiskās atbildes**).</span><span class="sxs-lookup"><span data-stu-id="38677-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="38677-108">**2. metode**</span><span class="sxs-lookup"><span data-stu-id="38677-108">**Method 2**</span></span>

1. <span data-ttu-id="38677-109">Pierakstieties Office 365 administrēšanas portālā, izmantojot administratora akreditācijas datus.</span><span class="sxs-lookup"><span data-stu-id="38677-109">Sign in to the Office 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="38677-110">Izvērsiet sadaļu **Administrēšanas centri** un pēc tam noklikšķiniet uz **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="38677-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="38677-111">Noklikšķiniet uz attēla augšējā labajā stūrī, noklikšķiniet uz **Cits lietotājs** un pēc tam atlasiet lietotāja pastkasti, kuru vēlaties mainīt.</span><span class="sxs-lookup"><span data-stu-id="38677-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="38677-112">Kreisajā pusē atlasiet **Opcijas**, noklikšķiniet uz **Organizēt e-pastu** un pēc tam uz **Automātiskās atbildes.**</span><span class="sxs-lookup"><span data-stu-id="38677-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="38677-113">**3. metode**</span><span class="sxs-lookup"><span data-stu-id="38677-113">**Method 3**</span></span>

<span data-ttu-id="38677-114">Izpildiet tālāk norādīto cmdlet programmā Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="38677-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="38677-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="38677-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="38677-116">Papildinformāciju par šo cmdlet komandu skatiet rakstā [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="38677-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
