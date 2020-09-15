---
title: Ārējo e-pasta pārsūtīšanas noteikšana uz pastkastēm audita žurnālos
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
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696304"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="a54cf-102">E-pasta pārsūtīšanas noteikšana pastkastēs</span><span class="sxs-lookup"><span data-stu-id="a54cf-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="a54cf-103">Ja Microsoft 365 lietotājs konfigurē ārējo e-pasta pārsūtīšanu pastkastē, darbība tiek auditēta kā daļa no **Set-Mailbox** cmdlet.</span><span class="sxs-lookup"><span data-stu-id="a54cf-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="a54cf-104">Varat skatīt aktivitāti, izmantojot audita žurnālu meklēšanu drošības & atbilstības centrā.</span><span class="sxs-lookup"><span data-stu-id="a54cf-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="a54cf-105">Piesakieties [Microsoft 365 drošības & atbilstības centrā](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="a54cf-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="a54cf-106">Dodieties **uz meklēšanas**  >  **audita žurnālu meklēšanas** lapā.</span><span class="sxs-lookup"><span data-stu-id="a54cf-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="a54cf-107">Atlasiet datumu diapazonu lauku **sākuma datums** un **beigšanas datums** .</span><span class="sxs-lookup"><span data-stu-id="a54cf-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="a54cf-108">Nav jānorāda lietotājvārds.</span><span class="sxs-lookup"><span data-stu-id="a54cf-108">You don't need to specify a username.</span></span> <span data-ttu-id="a54cf-109">Pārbaudiet, vai lauks **aktivitātes** ir iestatīts uz **Rādīt rezultātus visās aktivitātēs**.</span><span class="sxs-lookup"><span data-stu-id="a54cf-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="a54cf-110">Noklikšķiniet uz **Meklēt**.</span><span class="sxs-lookup"><span data-stu-id="a54cf-110">Click **Search**.</span></span>

<span data-ttu-id="a54cf-111">Rezultātos noklikšķiniet uz **filtrēt rezultātus** un ierakstiet **Set-pastkaste** lodziņā darbību filtrs.</span><span class="sxs-lookup"><span data-stu-id="a54cf-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="a54cf-112">Rezultātos atlasiet audita ierakstu.</span><span class="sxs-lookup"><span data-stu-id="a54cf-112">Select an audit record in the results.</span></span> <span data-ttu-id="a54cf-113">**Detalizētas** informācijas izlidošanas sarakstā noklikšķiniet uz **Papildinformācija**.</span><span class="sxs-lookup"><span data-stu-id="a54cf-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="a54cf-114">Jums ir jāaplūko detalizēta informācija par katru audita ierakstu, lai noteiktu, vai darbība ir saistīta ar e-pasta pārsūtīšanu.</span><span class="sxs-lookup"><span data-stu-id="a54cf-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="a54cf-115">**ObjectId**: modificētās pastkastes aizstājvārda vērtība.</span><span class="sxs-lookup"><span data-stu-id="a54cf-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="a54cf-116">**Parametri**: _ForwardingSmtpAddress_ norāda e-pasta adresi.</span><span class="sxs-lookup"><span data-stu-id="a54cf-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="a54cf-117">Lietotāja **ID**: lietotājs, kurš ir konfigurējis e-pasta pārsūtīšanu pastkastē **ObjectId** laukā.</span><span class="sxs-lookup"><span data-stu-id="a54cf-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="a54cf-118">Papildinformāciju skatiet rakstā [e-pasta pārsūtīšanas iestatīšana pastkastei](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="a54cf-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span></span>
