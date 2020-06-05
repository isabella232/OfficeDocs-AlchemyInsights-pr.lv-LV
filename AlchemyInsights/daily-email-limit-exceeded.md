---
title: Pārsniegts ikdienas e-pasta limits. Darbplūsma ir apturēta.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 701c4aef6bfc0c4a2c4570f6dd16dbe4f99efc44
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580340"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="a079e-103">Pārsniegts ikdienas e-pasta limits.</span><span class="sxs-lookup"><span data-stu-id="a079e-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="a079e-104">Darbplūsma ir apturēta.</span><span class="sxs-lookup"><span data-stu-id="a079e-104">Workflow is suspended.</span></span>

<span data-ttu-id="a079e-105">Šī kļūda var tikt saņemta šādos gadījumos:</span><span class="sxs-lookup"><span data-stu-id="a079e-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="a079e-106">Jums ir darbplūsma SharePoint Online, kas izmanto SharePoint 2010 vai SharePoint 2013 darbplūsmas platformas tips.</span><span class="sxs-lookup"><span data-stu-id="a079e-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="a079e-107">Darbplūsma ir konfigurēta, lai nosūtītu pielāgotu e-pasta ziņojumu vairāk nekā 200 lietotājiem laikā, vairāk nekā 10 000 adresāti dienā vai vairāk nekā 30 ziņojumi minūtē.</span><span class="sxs-lookup"><span data-stu-id="a079e-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="a079e-108">Palaižot darbplūsmu, e-pasta ziņojums netiek nosūtīts un pamanāt, ka šādas darbības:</span><span class="sxs-lookup"><span data-stu-id="a079e-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="a079e-109">Darbplūsmu, izmantojot SharePoint 2013 platformas tips, pārlūkojot lapu **darbplūsmas statuss** .</span><span class="sxs-lookup"><span data-stu-id="a079e-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="a079e-110">Lapā Darbplūsmas statuss **iekšējais statuss** ir iestatīts uz **sākts**un informācijas balons parāda **nevar nosūtīt adresātam**.</span><span class="sxs-lookup"><span data-stu-id="a079e-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="a079e-111">Lai novērstu šo problēmu, konfigurējiet darbplūsmas nosūtīt e-pasta ziņojumus, nepārsniedzot [Exchange Online sūtītāja ierobežojumus](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="a079e-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="a079e-112">Piemēram, izmantojiet pauzi darbplūsmā, nosūtiet e-pastu uz Microsoft 365 grupu, adresātu grupu vai iespējotu pasta drošības grupu vai arī nosūtiet ziņojumu mazāk nekā 200 adresātiem vienlaikus.</span><span class="sxs-lookup"><span data-stu-id="a079e-112">For example, use a pause in the workflow, send the email to a Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="a079e-113">Lai iegūtu papildinformāciju, skatiet šo [rakstu](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="a079e-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="a079e-114">Saistītās tēmas</span><span class="sxs-lookup"><span data-stu-id="a079e-114">Related topics</span></span>
- [<span data-ttu-id="a079e-115">Izveidot plūsmu</span><span class="sxs-lookup"><span data-stu-id="a079e-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="a079e-116">SharePoint un plūsmas</span><span class="sxs-lookup"><span data-stu-id="a079e-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 