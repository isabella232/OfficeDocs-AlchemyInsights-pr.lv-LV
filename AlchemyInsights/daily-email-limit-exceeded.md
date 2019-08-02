---
title: Ikdienas e-pasta limits pārsniegts. Darba plūsma tiks pārtraukta.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 802aba696da61be5f0a6c12072842cbc3cd96499
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059645"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="c7c9b-103">Ikdienas e-pastu pārsniegts.</span><span class="sxs-lookup"><span data-stu-id="c7c9b-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="c7c9b-104">Darba plūsma tiks pārtraukta.</span><span class="sxs-lookup"><span data-stu-id="c7c9b-104">Workflow is suspended.</span></span>

<span data-ttu-id="c7c9b-105">Šī kļūda var saņemt šādos gadījumos:</span><span class="sxs-lookup"><span data-stu-id="c7c9b-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="c7c9b-106">Darbplūsma ir SharePoint Online, kas izmanto SharePoint 2010 vai SharePoint 2013 darbplūsmas platformas tipa.</span><span class="sxs-lookup"><span data-stu-id="c7c9b-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="c7c9b-107">Darbplūsma ir konfigurēta, lai nosūtītu pielāgotus e-pasta ziņu vairāk nekā 200 lietotājiem laikā, vairāk nekā 10000 adresāti dienā vai vairāk nekā 30 ziņojumi minūtē.</span><span class="sxs-lookup"><span data-stu-id="c7c9b-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="c7c9b-108">Palaižot darbplūsmu, e-pasta ziņa nav nosūtīta un ievērojiet tālāk minētās darbības:</span><span class="sxs-lookup"><span data-stu-id="c7c9b-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="c7c9b-109">Darbplūsmu, izmantojot SharePoint 2013 platformas tipa, jūs pārlūkot lapu **Darbplūsmas statuss** .</span><span class="sxs-lookup"><span data-stu-id="c7c9b-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="c7c9b-110">Darbplūsmas statusa lapā **Iekšējais statuss** ir iestatīts uz **uzsākšana**un informācijas balons parāda **nevar nosūtīt adresātam**.</span><span class="sxs-lookup"><span data-stu-id="c7c9b-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="c7c9b-111">Lai apietu šo problēmu, konfigurējiet darbplūsmas nosūtīt e-pasta ziņojumus bez [Exchange Online sūtītāja robežas](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)pārsniegšana.</span><span class="sxs-lookup"><span data-stu-id="c7c9b-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="c7c9b-112">Piemēram, lietot darbplūsmas pauzi, nosūtīt e-pastu uz Office 365 grupu, adresātu grupu vai pasta iespējots drošības grupa vai nosūtītu ziņu uz mazāk nekā 200 adresātiem vienā reizē.</span><span class="sxs-lookup"><span data-stu-id="c7c9b-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="c7c9b-113">Lai iegūtu papildinformāciju, skatiet šādu [rakstu](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="c7c9b-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="c7c9b-114">Saistītās tēmas</span><span class="sxs-lookup"><span data-stu-id="c7c9b-114">Related topics</span></span>
- [<span data-ttu-id="c7c9b-115">Radīt plūsmu</span><span class="sxs-lookup"><span data-stu-id="c7c9b-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="c7c9b-116">SharePoint un plūsmas</span><span class="sxs-lookup"><span data-stu-id="c7c9b-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 