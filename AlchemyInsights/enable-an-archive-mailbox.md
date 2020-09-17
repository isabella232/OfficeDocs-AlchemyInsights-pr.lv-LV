---
title: Arhīva pastkastes iespējošana
ms.author: markjjo
author: markjjo
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "307"
- "3100008"
ms.assetid: e1a5fab7-d3a5-4d4c-8ee2-0edf4ec9b76b
ms.openlocfilehash: 3e20eaf8dec85454ce5a67e1b21292b2a33ebb1d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47811712"
---
# <a name="enable-an-archive-mailbox"></a><span data-ttu-id="a0161-102">Arhīva pastkastes iespējošana</span><span class="sxs-lookup"><span data-stu-id="a0161-102">Enable an archive mailbox</span></span>

<span data-ttu-id="a0161-103">Ja vēlaties, lai mēs veiktu automatizētās pārbaudes, lai nodrošinātu, ka arhīva pastkasti var konfigurēt, atlasiet pogu atpakaļ < — šīs lapas augšdaļā un pēc tam ievadiet konta e-pasta adresi.</span><span class="sxs-lookup"><span data-stu-id="a0161-103">If you want us to run automated checks to ensure an archive mailbox can be configured, select the back button <-- at the top of this page, and then enter the email address of the account.</span></span>

<span data-ttu-id="a0161-104">Arhivēt pastkastes pakalpojumā Microsoft 365 (ko dēvē arī par *tiešsaistes arhīvu* vai *oriģinālu arhīvu*) nodrošina lietotājiem papildu e-pasta krātuvi.</span><span class="sxs-lookup"><span data-stu-id="a0161-104">Archive mailboxes in Microsoft 365 (also called *Online Archives* or *In-Place Archives*) provide users with additional email storage.</span></span> <span data-ttu-id="a0161-105">Lietotāji var pārvietot vai kopēt vienumus uz arhīva pastkasti, un administratori var izveidot arhīva politiku, kas automātiski pārvieto vienumus uz arhīva pastkastēm.</span><span class="sxs-lookup"><span data-stu-id="a0161-105">Users can move or copy items to their archive mailbox, and admins can create an archive policy that automatically moves items to archive mailboxes.</span></span>
  
<span data-ttu-id="a0161-106">Tālāk ir aprakstīts, kā izveidot arhīva pastkasti.</span><span class="sxs-lookup"><span data-stu-id="a0161-106">Here's how to create an archive mailbox:</span></span>
  
1. <span data-ttu-id="a0161-107">Dodieties uz [https://protection.office.com](https://protection.office.com) .</span><span class="sxs-lookup"><span data-stu-id="a0161-107">Go to [https://protection.office.com](https://protection.office.com).</span></span>

2. <span data-ttu-id="a0161-108">Pierakstieties pakalpojumā Microsoft 365, izmantojot savu administratora kontu.</span><span class="sxs-lookup"><span data-stu-id="a0161-108">Sign in to Microsoft 365 using your admin account.</span></span>

3. <span data-ttu-id="a0161-109">Drošības &amp; atbilstības centra kreisajā rūtī atlasiet **informācijas pārvaldības** \> **Arhīvs**.</span><span class="sxs-lookup"><span data-stu-id="a0161-109">In the left pane of the Security &amp; Compliance Center, select **Information governance** \> **Archive**.</span></span>

4. <span data-ttu-id="a0161-110">Atlasiet lietotāju, kura arhīva pastkasti vēlaties iespējot.</span><span class="sxs-lookup"><span data-stu-id="a0161-110">Select the user whose archive mailbox you want to enable.</span></span>

5. <span data-ttu-id="a0161-111">Detalizētās informācijas rūtī pa labi noklikšķiniet uz **Iespējot** un pēc tam brīdinājuma ziņojumā noklikšķiniet uz **Jā** , lai iespējotu arhīva pastkasti.</span><span class="sxs-lookup"><span data-stu-id="a0161-111">In the details pane on the right, click **Enable** and then click **Yes** in the warning message to enable the archive mailbox.</span></span>

<span data-ttu-id="a0161-112">Varat arī veikt lielapjoma arhīva pastkastu iespējošanu, atlasot vairākus lietotājus (izmantojot **taustiņu SHIFT** vai **CTRL** ) un pēc tam detalizētās informācijas rūtī noklikšķinot uz **Iespējot** .</span><span class="sxs-lookup"><span data-stu-id="a0161-112">You can also bulk-enable archive mailboxes by selecting multiple users (using the **Shift** or **Ctrl** keys) and then clicking **Enable** in the details pane.</span></span>
  
### <a name="shared-mailboxes"></a><span data-ttu-id="a0161-113">Koplietojamas pastkastes</span><span class="sxs-lookup"><span data-stu-id="a0161-113">Shared mailboxes</span></span>

<span data-ttu-id="a0161-114">Lai iespējotu koplietojamas pastkastes arhīvu, ir nepieciešama Exchange Online plāna 2 licence vai Exchange Online 1. plāns, kurā ir iekļauta Exchange Online arhivēšanas licence.</span><span class="sxs-lookup"><span data-stu-id="a0161-114">To enable the archive for a shared mailbox, an Exchange Online Plan 2 license or an Exchange Online Plan 1 license with an Exchange Online Archiving license is required.</span></span>  

<span data-ttu-id="a0161-115">Lai iespējotu koplietojamas pastkastes arhīvu:</span><span class="sxs-lookup"><span data-stu-id="a0161-115">To enable the archive for a shared mailbox:</span></span>

1. <span data-ttu-id="a0161-116">Dodieties uz [Exchange administrēšanas centru](https://outlook.office365.com/ecp) un pierakstieties, izmantojot savu administratora kontu.</span><span class="sxs-lookup"><span data-stu-id="a0161-116">Go to the [Exchange admin center](https://outlook.office365.com/ecp) and sign in using your admin account.</span></span>

2. <span data-ttu-id="a0161-117">Dodieties uz **Recipients**  >  **kopīgotie**adresāti.</span><span class="sxs-lookup"><span data-stu-id="a0161-117">Go to **Recipients** > **Shared**.</span></span>

3. <span data-ttu-id="a0161-118">Atlasiet koplietojamo pastkasti.</span><span class="sxs-lookup"><span data-stu-id="a0161-118">Select the shared mailbox.</span></span>

4. <span data-ttu-id="a0161-119">Detalizētās informācijas rūtī labajā pusē zem lokālās **arhīva**noklikšķiniet uz **Iespējot**un pēc tam uz **Jā** , lai iespējotu arhīva pastkasti.</span><span class="sxs-lookup"><span data-stu-id="a0161-119">In the details pane on the right, under **In-Place Archive**, click **Enable**, and then click **Yes** to enable the archive mailbox.</span></span>

<span data-ttu-id="a0161-120">Papildinformāciju skatiet rakstā:</span><span class="sxs-lookup"><span data-stu-id="a0161-120">For more information, see:</span></span>
  
- [<span data-ttu-id="a0161-121">Arhīva pastkastu iespējošana</span><span class="sxs-lookup"><span data-stu-id="a0161-121">Enable archive mailboxes</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes)

- [<span data-ttu-id="a0161-122">Arhivēšanas un dzēšanas politikas iestatīšana</span><span class="sxs-lookup"><span data-stu-id="a0161-122">Set up an archive and deletion policy</span></span>](https://docs.microsoft.com//office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes)
