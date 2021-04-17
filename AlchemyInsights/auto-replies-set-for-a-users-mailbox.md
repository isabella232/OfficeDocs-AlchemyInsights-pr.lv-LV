---
title: Automātisko atbilžu iestatīšana pastkastē
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 60af581e7fe508ab9644a53873bcd551b3aacff1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820941"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="a35a1-102">Automātisko atbilžu iestatīšana lietotāja pastkastē</span><span class="sxs-lookup"><span data-stu-id="a35a1-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="a35a1-103">**1. metode**</span><span class="sxs-lookup"><span data-stu-id="a35a1-103">**Method 1**</span></span>

1. <span data-ttu-id="a35a1-104">Pierakstieties programmas Microsoft 365 portālā.</span><span class="sxs-lookup"><span data-stu-id="a35a1-104">Sign in to the Microsoft 365 portal.</span></span>

2. <span data-ttu-id="a35a1-105">Dodieties uz **Lietotāji > Aktīvie lietotāji** (vai **Grupas > Koplietojamās pastkastes**, ja esat iestatījis šo kā koplietojamo pastkasti).</span><span class="sxs-lookup"><span data-stu-id="a35a1-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="a35a1-106">Atlasiet lietotāju, kuram ir Microsoft Exchange pastkaste.</span><span class="sxs-lookup"><span data-stu-id="a35a1-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="a35a1-107">Uznirstošajā izvēlnē labajā pusē dodieties uz **Pasta iestatījumi > Automātiskās atbildes** (ja tā ir koplietojama pastkaste, vienkārši izvēlnē noklikšķiniet uz **Automātiskās atbildes**).</span><span class="sxs-lookup"><span data-stu-id="a35a1-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="a35a1-108">**2. metode**</span><span class="sxs-lookup"><span data-stu-id="a35a1-108">**Method 2**</span></span>

1. <span data-ttu-id="a35a1-109">Pierakstieties Microsoft 365 administrēšanas portālā, izmantojot administratora akreditācijas datus.</span><span class="sxs-lookup"><span data-stu-id="a35a1-109">Sign in to the Microsoft 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="a35a1-110">Izvērsiet sadaļu **Administrēšanas centri** un pēc tam noklikšķiniet uz **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="a35a1-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="a35a1-111">Noklikšķiniet uz attēla augšējā labajā stūrī, noklikšķiniet uz **Cits lietotājs** un pēc tam atlasiet lietotāja pastkasti, kuru vēlaties mainīt.</span><span class="sxs-lookup"><span data-stu-id="a35a1-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="a35a1-112">Kreisajā pusē atlasiet **Opcijas**, noklikšķiniet uz **Organizēt e-pastu** un pēc tam uz **Automātiskās atbildes.**</span><span class="sxs-lookup"><span data-stu-id="a35a1-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="a35a1-113">**3. metode**</span><span class="sxs-lookup"><span data-stu-id="a35a1-113">**Method 3**</span></span>

<span data-ttu-id="a35a1-114">Izpildiet tālāk norādīto cmdlet programmā Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="a35a1-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="a35a1-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="a35a1-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="a35a1-116">Papildinformāciju par šo cmdlet komandu skatiet rakstā [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="a35a1-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
