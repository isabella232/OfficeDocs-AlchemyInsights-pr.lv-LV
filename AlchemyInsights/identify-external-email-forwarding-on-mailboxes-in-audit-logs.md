---
title: Identificēt ārējiem e-pasta pāradresācija uz pastkastēm, audita žurnālos
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 7fb2c161c558a7eb961f86ca2b86e33750d902fd
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/23/2019
ms.locfileid: "32417218"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="aa2e0-102">Noteikt, kad ir konfigurēta ārējiem e-pasta pāradresācija pastkastēm</span><span class="sxs-lookup"><span data-stu-id="aa2e0-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="aa2e0-103">Kad lietotājs konfigurē ārējiem e-pasta pāradresācija uz pastkasti, darbība tiek veikta revīzija, kā daļa no **Kopas-Mailbox** cmdlet.</span><span class="sxs-lookup"><span data-stu-id="aa2e0-103">When a user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="aa2e0-104">Jūs varat redzēt, izmantojot audita žurnālu meklēšana drošības & Center izpildes darbības.</span><span class="sxs-lookup"><span data-stu-id="aa2e0-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="aa2e0-105">[Office drošības 365 & atbilstību centra](https://protection.office.com/) pieteikties</span><span class="sxs-lookup"><span data-stu-id="aa2e0-105">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="aa2e0-106">Noklikšķiniet uz **meklēšanas un izmeklēšanas** un atlasiet **Audita žurnālu meklēšana**.</span><span class="sxs-lookup"><span data-stu-id="aa2e0-106">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="aa2e0-107">Atlasiet datumu diapazona **sākuma datums** un **beigu datums** laukos.</span><span class="sxs-lookup"><span data-stu-id="aa2e0-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="aa2e0-108">Jums nav nepieciešams norādīt lietotājvārdu.</span><span class="sxs-lookup"><span data-stu-id="aa2e0-108">You don't need to specify a username.</span></span> <span data-ttu-id="aa2e0-109">Pārbaudīt **darbības** lauks ir iestatīts uz **Parādīt visas darbības rezultātus**.</span><span class="sxs-lookup"><span data-stu-id="aa2e0-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="aa2e0-110">Noklikšķiniet uz **Meklēt**.</span><span class="sxs-lookup"><span data-stu-id="aa2e0-110">Click **Search**.</span></span>

<span data-ttu-id="aa2e0-111">Rezultātos, noklikšķiniet uz **Filtrēt rezultātus** un darbības filtrs lodziņā ierakstiet **Set pastkastes** .</span><span class="sxs-lookup"><span data-stu-id="aa2e0-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="aa2e0-112">Atlasiet ierakstu audita rezultātiem.</span><span class="sxs-lookup"><span data-stu-id="aa2e0-112">Select an audit record in the results.</span></span> <span data-ttu-id="aa2e0-113">Flyout **detaļas** , noklikšķiniet uz **Papildinformācija**.</span><span class="sxs-lookup"><span data-stu-id="aa2e0-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="aa2e0-114">Jums ir aplūkot detalizētu informāciju par katru audita ierakstu, lai noteiktu, ja darbība ir saistīta ar e-pasta pāradresācija.</span><span class="sxs-lookup"><span data-stu-id="aa2e0-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="aa2e0-115">**ObjectId**: aizstājvārds vērtība pastkasti, kura tika modificēta.</span><span class="sxs-lookup"><span data-stu-id="aa2e0-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="aa2e0-116">**Parametri**: _ForwardingSmtpAddress_ norāda mērķa e-pasta adresi.</span><span class="sxs-lookup"><span data-stu-id="aa2e0-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="aa2e0-117">**UserId**: lietotāju, kas ir konfigurēta e-pasta pāradresāciju uz **ObjectId** laukā pastkastes.</span><span class="sxs-lookup"><span data-stu-id="aa2e0-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="aa2e0-118">Plašāku informāciju skatiet [noteikšana, kas izveido e-pasta pāradresācija uz pastkasti](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="aa2e0-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
