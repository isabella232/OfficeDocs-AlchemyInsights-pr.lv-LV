---
title: Automātiska ar konkrētiem domēniem sūtīto Office 365 e-pasta ziņojumu šifrēšana
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
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526690"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a><span data-ttu-id="67c83-102">Automātiska ar konkrētiem domēniem sūtīto Office 365 e-pasta ziņojumu šifrēšana</span><span class="sxs-lookup"><span data-stu-id="67c83-102">Automatically encrypt Office 365 email messages sent to certain domains</span></span>

1. <span data-ttu-id="67c83-103">[Exchange administrēšanas centrā](https://outlook.office365.com/ecp/)izvēlieties **pasta plūsmas > kārtulas**.</span><span class="sxs-lookup"><span data-stu-id="67c83-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="67c83-104">Noklikšķiniet uz **jaunās (+)** ikonas un pēc tam noklikšķiniet uz **lietot Office 365 ziņojumu šifrēšanu un tiesību aizsardzību uz ziņojumiem**.</span><span class="sxs-lookup"><span data-stu-id="67c83-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="67c83-105">Lodziņā **nosaukums** ievadiet kārtulas nosaukumu, piemēram, *šifrētu ziņojumus, kas nosūtīti uz contoso.com*.</span><span class="sxs-lookup"><span data-stu-id="67c83-105">In **Name**, enter a name for the rule, such as *Encrypt messages sent to contoso.com*.</span></span>
4. <span data-ttu-id="67c83-106">Sadaļā **lietot šo kārtulu, ja** izvēlieties **adresātu > domēns**.</span><span class="sxs-lookup"><span data-stu-id="67c83-106">In **Apply this rule if**, choose **The recipient > domain is**.</span></span> 
5. <span data-ttu-id="67c83-107">Ievadiet tā domēna nosaukumu, piemēram, **contoso.com**.</span><span class="sxs-lookup"><span data-stu-id="67c83-107">Enter the name of the domain, such as **contoso.com**.</span></span>
6. <span data-ttu-id="67c83-108">Noklikšķiniet uz ikonas **Add (+)** un pēc tam noklikšķiniet uz **Labi**.</span><span class="sxs-lookup"><span data-stu-id="67c83-108">Click the **Add (+)** icon, and then click **OK**.</span></span>
7. <span data-ttu-id="67c83-109">Blakus **veikt tālāk norādītās** darbības noklikšķiniet uz **Atlasīt vienu**.</span><span class="sxs-lookup"><span data-stu-id="67c83-109">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="67c83-110">**RMS veidnes** nolaižamajā izvēlnē atlasiet **Šifrēt** un pēc tam noklikšķiniet uz **Labi**.</span><span class="sxs-lookup"><span data-stu-id="67c83-110">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="67c83-111">(Ja neredzat šo opciju, tas nozīmē, ka jūsu plānā nav iekļauta automātiskā šifrēšana.</span><span class="sxs-lookup"><span data-stu-id="67c83-111">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="67c83-112">Taču jūs varat to pievienot!)</span><span class="sxs-lookup"><span data-stu-id="67c83-112">But you can add it!)</span></span>
9. <span data-ttu-id="67c83-113">Izvēlieties jebkuru neobligātu atlasi (no neobligāto atlases saraksta, ko varat veikt šajā brīdī, no kuriem daudzus var atstāt ar noklusējuma iestatījumu vienkāršībai).</span><span class="sxs-lookup"><span data-stu-id="67c83-113">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="67c83-114">Noklikšķiniet uz **Saglabāt**.</span><span class="sxs-lookup"><span data-stu-id="67c83-114">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="67c83-115">Vienmēr varat atgriezties un rediģēt šo kārtulu vēlāk.</span><span class="sxs-lookup"><span data-stu-id="67c83-115">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="67c83-116">Papildinformāciju par šifrēšanas kārtulu izveidi skatiet rakstā [pasta plūsmas kārtulu definēšana, lai šifrētu e-pasta ziņojumus pakalpojumā Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="67c83-116">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>