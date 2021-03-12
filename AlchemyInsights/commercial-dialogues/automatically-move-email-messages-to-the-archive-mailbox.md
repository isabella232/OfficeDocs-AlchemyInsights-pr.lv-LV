---
title: Automātiska e-pasta ziņojumu pārvietošana uz arhīva pastkasti
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746045"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a><span data-ttu-id="9b9c7-102">Automātiska e-pasta ziņojumu pārvietošana uz arhīva pastkasti</span><span class="sxs-lookup"><span data-stu-id="9b9c7-102">Automatically move email messages to the archive mailbox</span></span>

<span data-ttu-id="9b9c7-103">Tālāk ir aprakstīts, kā iestatīt politiku, lai automātiski pārvietotu lietotāja veco e-pasta ziņojumu uz arhīva pastkasti.</span><span class="sxs-lookup"><span data-stu-id="9b9c7-103">Here's how to set up a policy to automatically move a user's old email to the archive mailbox:</span></span>

1. <span data-ttu-id="9b9c7-104">Dodieties uz [**drošības & atbilstības**](https://go.microsoft.com/fwlink/p/?linkid=2077143)  >  **datu pārvaldības**  >  **arhīvu** , lai pārbaudītu, vai ir iespējota arhīva pastkaste lietotājam.</span><span class="sxs-lookup"><span data-stu-id="9b9c7-104">Go to [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **Data governance** > **Archive** to verify an archive mailbox has been enabled for the user.</span></span> <span data-ttu-id="9b9c7-105">Ja tā nav, brīdinājuma lodziņā noklikšķiniet uz **Iespējot** un pēc tam uz **Jā** .</span><span class="sxs-lookup"><span data-stu-id="9b9c7-105">If it hasn't, click **Enable** then **Yes** in the warning box.</span></span>
2. <span data-ttu-id="9b9c7-106">Dodieties uz [**Exchange administrēšanas centrs > atbilstības pārvaldības > saglabāšanas atzīmes**](https://go.microsoft.com/fwlink/?linkid=2059104).</span><span class="sxs-lookup"><span data-stu-id="9b9c7-106">Go to [**Exchange admin center > compliance management > retention tags**](https://go.microsoft.com/fwlink/?linkid=2059104).</span></span>
3. <span data-ttu-id="9b9c7-107">Izvēlieties ikonu +, pēc tam izvēlieties **automātiski lietot visai pastkastei**.</span><span class="sxs-lookup"><span data-stu-id="9b9c7-107">Choose the + icon then choose **automatically apply to entire mailbox**.</span></span>
4. <span data-ttu-id="9b9c7-108">Piešķiriet nosaukumu saglabāšanas frāzei un izvēlieties **Pārvietot uz arhīvu**.</span><span class="sxs-lookup"><span data-stu-id="9b9c7-108">Assign a name to the retention tag, and choose **Move to Archive**.</span></span> <span data-ttu-id="9b9c7-109">Saglabāšanas periodam ievadiet vēlamo laiku, piemēram, 90 dienas.</span><span class="sxs-lookup"><span data-stu-id="9b9c7-109">For the retention period, enter the time you want, such as 90 days.</span></span> <span data-ttu-id="9b9c7-110">Noklikšķiniet uz **Saglabāt**.</span><span class="sxs-lookup"><span data-stu-id="9b9c7-110">Click **Save**.</span></span>
5. <span data-ttu-id="9b9c7-111">Tagad izveidojiet saglabāšanas politiku: izvēlieties **saglabāšanas** politikas, izvēlieties ikonu, lai pievienotu jaunu politiku.</span><span class="sxs-lookup"><span data-stu-id="9b9c7-111">Now create a retention policy: choose **retention policies**, choose the icon to add a new policy.</span></span>
6. <span data-ttu-id="9b9c7-112">Piešķiriet nosaukumu saglabāšanas politikai, pēc tam noklikšķiniet un ritiniet, lai atrastu un pievienotu saglabāšanas atzīmi, ko tikko izveidojāt.</span><span class="sxs-lookup"><span data-stu-id="9b9c7-112">Assign a name to the retention policy, then click and scroll to find and add the retention tag you just created.</span></span> <span data-ttu-id="9b9c7-113">Noklikšķiniet uz **Saglabāt**.</span><span class="sxs-lookup"><span data-stu-id="9b9c7-113">Click **Save**.</span></span>
7. <span data-ttu-id="9b9c7-114">Visbeidzot, lietotāja pastkastei lietojiet saglabāšanas politiku: joprojām Exchange administrēšanas centrā dodieties uz **adresāti**  >  **pastkastes**.</span><span class="sxs-lookup"><span data-stu-id="9b9c7-114">Finally, apply the retention policy to the user's mailbox: still in the Exchange admin center, go to **recipients** > **mailboxes**.</span></span> <span data-ttu-id="9b9c7-115">Izvēlieties visi lietotāji, kuriem vēlaties lietot politiku, un pēc tam izvēlieties **Rediģēt** (zīmuļa ikona).</span><span class="sxs-lookup"><span data-stu-id="9b9c7-115">Choose all the users who you want to apply the policy to, then choose **Edit** (the pencil icon).</span></span>
8. <span data-ttu-id="9b9c7-116">Dialoglodziņā noklikšķiniet uz **pastkastes līdzekļi**.</span><span class="sxs-lookup"><span data-stu-id="9b9c7-116">In the dialog box, click **mailbox features**.</span></span> <span data-ttu-id="9b9c7-117">Sadaļā **saglabāšanas politika** lietojiet tikko izveidoto politiku > **Saglabāt**.</span><span class="sxs-lookup"><span data-stu-id="9b9c7-117">Under **Retention policy**, apply the policy you just created > **Save**.</span></span>
9. <span data-ttu-id="9b9c7-118">Norādījumus par politikas lietošanu visiem lietotājiem skatiet rakstā [saglabāšanas politikas lietošana pastkastēm](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span><span class="sxs-lookup"><span data-stu-id="9b9c7-118">For instructions for applying the policy to all users, see [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span></span>
