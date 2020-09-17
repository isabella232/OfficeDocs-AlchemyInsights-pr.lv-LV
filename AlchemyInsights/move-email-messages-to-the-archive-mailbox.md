---
title: E-pasta ziņojumu pārvietošana uz arhīva pastkasti
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799787"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="b0673-102">E-pasta pārvietošana uz arhīva pastkasti</span><span class="sxs-lookup"><span data-stu-id="b0673-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="b0673-103">Ja vēlaties, lai mēs veiktu automatizētās pārbaudes par tālāk norādītajiem iestatījumiem, atlasiet pogu atpakaļ < — šīs lapas augšdaļā un pēc tam ievadiet tā lietotāja e-pasta adresi, kuram ir problēmas ar e-pasta pārvietošanu uz viņu arhīva pastkasti.</span><span class="sxs-lookup"><span data-stu-id="b0673-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="b0673-104">Apstipriniet, ka **arhīva pastkaste** ir iespējota.</span><span class="sxs-lookup"><span data-stu-id="b0673-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="b0673-105">Ja ne, veiciet [šajā rakstā](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) norādītās darbības, lai iespējotu arhīva pastkasti.</span><span class="sxs-lookup"><span data-stu-id="b0673-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="b0673-106">Lai automātiski arhivētu ziņojumus arhīva pastkastei, saglabāšanas tagam ar darbību **Pārvietot uz arhivēšanu** ir jāiestata **automātiski lietot visam pastkastes (noklusējuma) tagam**.</span><span class="sxs-lookup"><span data-stu-id="b0673-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="b0673-107">Veiciet šeit norādītās darbības, lai izveidotu atzīmi: [Arhivēt noklusējuma atzīmi](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="b0673-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="b0673-108">Pēc tam pievienojiet **arhīva** atzīmi savam saglabāšanas politikai.</span><span class="sxs-lookup"><span data-stu-id="b0673-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="b0673-109">Exchange administrēšanas centrā izvēlieties **saglabāšanas politikas** > pievienot **pāriešanai uz arhīva atzīmi** politikas > **Saglabāt**.</span><span class="sxs-lookup"><span data-stu-id="b0673-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="b0673-110">Tagad [Piešķiriet saglabāšanas politiku](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) konkrētam lietotāja pastkastei.</span><span class="sxs-lookup"><span data-stu-id="b0673-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="b0673-111">Viena un tā pati politika tiek lietota gan **primārajai** , gan **arhīva** pastkastei.</span><span class="sxs-lookup"><span data-stu-id="b0673-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="b0673-112">Iespējams, ka ir jāspiež pārvaldītā mapes asistents (MFA), lai palaistu un lietotu jaunos iestatījumus lietotāja pastkastē.</span><span class="sxs-lookup"><span data-stu-id="b0673-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="b0673-113">Izpildiet šādu komandu, kamēr ir [izveidots savienojums ar EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) , lai startētu pārvaldīto mapju palīgu noteiktai pastkastei.</span><span class="sxs-lookup"><span data-stu-id="b0673-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="b0673-114">Start-ManagedFolderAssistant-Identity <name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="b0673-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="b0673-115">Papildinformāciju par arhīva politikas iestatīšanu skatiet rakstā [arhivēšanas un dzēšanas politikas iestatīšana pastkastēm](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="b0673-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  