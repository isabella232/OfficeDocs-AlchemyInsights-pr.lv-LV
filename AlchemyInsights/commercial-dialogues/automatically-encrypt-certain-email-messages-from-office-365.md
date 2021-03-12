---
title: Noteiktu e-pasta ziņojumu automātiska šifrēšana pakalpojumā Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746132"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a><span data-ttu-id="c8be3-102">Noteiktu e-pasta ziņojumu automātiska šifrēšana pakalpojumā Office 365</span><span class="sxs-lookup"><span data-stu-id="c8be3-102">Automatically encrypt certain email messages from office 365</span></span>

1. <span data-ttu-id="c8be3-103">[Exchange administrēšanas centrā](https://outlook.office365.com/ecp/)izvēlieties **pasta plūsmas > kārtulas**.</span><span class="sxs-lookup"><span data-stu-id="c8be3-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="c8be3-104">Noklikšķiniet uz **jaunās (+)** ikonas un pēc tam noklikšķiniet uz **lietot Office 365 ziņojumu šifrēšanu un tiesību aizsardzību uz ziņojumiem**.</span><span class="sxs-lookup"><span data-stu-id="c8be3-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="c8be3-105">Lodziņā **nosaukums** ievadiet kārtulas nosaukumu, piemēram, *visu ziņojumu šifrēšanu*.</span><span class="sxs-lookup"><span data-stu-id="c8be3-105">In **Name**, enter a name for the rule, such as *Encrypt all messages*.</span></span>
4. <span data-ttu-id="c8be3-106">Sadaļā **lietot šo kārtulu, ja** izvēlieties **[lietot visiem ziņojumiem]**.</span><span class="sxs-lookup"><span data-stu-id="c8be3-106">In **Apply this rule if**, choose **[Apply to all messages]**.</span></span> 
5. <span data-ttu-id="c8be3-107">Blakus **veikt tālāk norādītās** darbības noklikšķiniet uz **Atlasīt vienu**.</span><span class="sxs-lookup"><span data-stu-id="c8be3-107">Next to the **Do the following** field, click **Select one**.</span></span> 
6. <span data-ttu-id="c8be3-108">**RMS veidnes** nolaižamajā izvēlnē atlasiet **Šifrēt** un pēc tam noklikšķiniet uz **Labi**.</span><span class="sxs-lookup"><span data-stu-id="c8be3-108">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="c8be3-109">(Ja neredzat šo opciju, tas nozīmē, ka jūsu plānā nav iekļauta automātiskā šifrēšana.</span><span class="sxs-lookup"><span data-stu-id="c8be3-109">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="c8be3-110">Taču jūs varat to pievienot!)</span><span class="sxs-lookup"><span data-stu-id="c8be3-110">But you can add it!)</span></span>
7. <span data-ttu-id="c8be3-111">Atzīmējiet izvēles rūtiņu **auditēt šo kārtulu ar nopietnības līmeni** un pēc tam atlasiet vēlamo līmeni.</span><span class="sxs-lookup"><span data-stu-id="c8be3-111">Check the **Audit this rule with severity level** check box, and then select the desired level.</span></span> <span data-ttu-id="c8be3-112">Ja jūsu uzņēmumam ir līgumsaistības par visu šifrēto e-pasta ziņojumu sūtīšanu, iesakām līmeni iestatīt kā **augstu**.</span><span class="sxs-lookup"><span data-stu-id="c8be3-112">If your company has contractual obligations to send all emails encrypted, I recommend setting the level to **High**.</span></span>
8. <span data-ttu-id="c8be3-113">Sadaļā **Izvēlieties šīs kārtulas modeli** noklikšķiniet uz **izpildīt**.</span><span class="sxs-lookup"><span data-stu-id="c8be3-113">Under **Choose a model for this rule**, click **Enforce**.</span></span> 
9. <span data-ttu-id="c8be3-114">Izvēlieties jebkuru neobligātu atlasi (no neobligāto atlases saraksta, ko varat veikt šajā brīdī, no kuriem daudzus var atstāt ar noklusējuma iestatījumu vienkāršībai).</span><span class="sxs-lookup"><span data-stu-id="c8be3-114">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="c8be3-115">Noklikšķiniet uz **Saglabāt**.</span><span class="sxs-lookup"><span data-stu-id="c8be3-115">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="c8be3-116">Vienmēr varat atgriezties un rediģēt šo kārtulu vēlāk.</span><span class="sxs-lookup"><span data-stu-id="c8be3-116">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="c8be3-117">Papildinformāciju par šifrēšanas kārtulu izveidi skatiet rakstā [pasta plūsmas kārtulu definēšana, lai šifrētu e-pasta ziņojumus pakalpojumā Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="c8be3-117">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>

