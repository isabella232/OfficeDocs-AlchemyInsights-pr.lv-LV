---
title: Noteiktu Office 365 e-pasta ziņojumu automātiska šifrēšana
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
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746129"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a><span data-ttu-id="c8530-102">Noteiktu Office 365 e-pasta ziņojumu automātiska šifrēšana</span><span class="sxs-lookup"><span data-stu-id="c8530-102">Automatically encrypt certain Office 365 email messages</span></span>

<span data-ttu-id="c8530-103">Varat automātiski šifrēt ziņojumus, ko lietotāji nosūta noteiktām ārējām personām vai organizācijām.</span><span class="sxs-lookup"><span data-stu-id="c8530-103">You can automatically encrypt messages that users send to certain external people or organizations.</span></span> <span data-ttu-id="c8530-104">Lai to izdarītu, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="c8530-104">To do this, perform the following steps:</span></span>

1. <span data-ttu-id="c8530-105">[Exchange administrēšanas centrā](https://outlook.office365.com/ecp/)izvēlieties **pasta plūsmas > kārtulas**.</span><span class="sxs-lookup"><span data-stu-id="c8530-105">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="c8530-106">Noklikšķiniet uz **jaunās (+)** ikonas un pēc tam noklikšķiniet uz **lietot Office 365 ziņojumu šifrēšanu un tiesību aizsardzību uz ziņojumiem**.</span><span class="sxs-lookup"><span data-stu-id="c8530-106">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="c8530-107">Lodziņā **nosaukums** ievadiet kārtulas nosaukumu, piemēram, *šifrētu ziņojumus, kas nosūtīti uz DrToniRamos@gmail.com*.</span><span class="sxs-lookup"><span data-stu-id="c8530-107">In **Name**, enter a name for the rule, such as *Encrypt messages sent to DrToniRamos@gmail.com*.</span></span>
4. <span data-ttu-id="c8530-108">Sadaļā **lietot šo kārtulu, ja** izvēlieties **adresātu > ir šī persona**.</span><span class="sxs-lookup"><span data-stu-id="c8530-108">In **Apply this rule if**, choose **The recipient > is this person**.</span></span> 
5. <span data-ttu-id="c8530-109">Logā **dalībnieku atlase** atlasiet tās personas vārdu, kurai vēlaties lietot šifrēšanas kārtulu, un pēc tam noklikšķiniet uz **Pievienot**.</span><span class="sxs-lookup"><span data-stu-id="c8530-109">In the **Select Members** window, select the name of the person you want the encryption rule to apply to, and then click **add**.</span></span> 
6. <span data-ttu-id="c8530-110">Kad lietotāji ir pievienoti, noklikšķiniet uz **Labi**.</span><span class="sxs-lookup"><span data-stu-id="c8530-110">When you're done adding users, click **OK**.</span></span>
7. <span data-ttu-id="c8530-111">Blakus **veikt tālāk norādītās** darbības noklikšķiniet uz **Atlasīt vienu**.</span><span class="sxs-lookup"><span data-stu-id="c8530-111">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="c8530-112">**RMS veidnes** nolaižamajā izvēlnē atlasiet **Šifrēt** un pēc tam noklikšķiniet uz **Labi**.</span><span class="sxs-lookup"><span data-stu-id="c8530-112">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="c8530-113">(Ja neredzat šo opciju, tas nozīmē, ka jūsu plānā nav iekļauta automātiskā šifrēšana.</span><span class="sxs-lookup"><span data-stu-id="c8530-113">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="c8530-114">Taču jūs varat to pievienot!)</span><span class="sxs-lookup"><span data-stu-id="c8530-114">But you can add it!)</span></span>
9. <span data-ttu-id="c8530-115">Izvēlieties jebkuru neobligātu atlasi (no neobligāto atlases saraksta, ko varat veikt šajā brīdī, no kuriem daudzus var atstāt ar noklusējuma iestatījumu vienkāršībai).</span><span class="sxs-lookup"><span data-stu-id="c8530-115">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="c8530-116">Noklikšķiniet uz **Saglabāt**.</span><span class="sxs-lookup"><span data-stu-id="c8530-116">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="c8530-117">Vienmēr varat atgriezties un rediģēt šo kārtulu vēlāk.</span><span class="sxs-lookup"><span data-stu-id="c8530-117">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="c8530-118">Papildinformāciju par šifrēšanas kārtulu veidošanu skatiet rakstā [pasta plūsmas kārtulu definēšana, lai šifrētu e-pasta ziņojumus pakalpojumā Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span><span class="sxs-lookup"><span data-stu-id="c8530-118">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

