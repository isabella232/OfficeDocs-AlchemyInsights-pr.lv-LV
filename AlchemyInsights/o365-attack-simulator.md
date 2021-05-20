---
title: 2681 attack simulator in Microsoft 365
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
- "2681"
ms.assetid: ''
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545733"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="aba83-102">Attack Simulator in Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="aba83-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="aba83-103">Vai trūkst uzbrukuma simulatora?</span><span class="sxs-lookup"><span data-stu-id="aba83-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="aba83-104">Uzbrukuma simulatoram ir **nepieciešama programmatūra Microsoft Defender Office 365 2.** vai Office 365 Enterprise **E5.**</span><span class="sxs-lookup"><span data-stu-id="aba83-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="aba83-105">Attack Simulator nav **iekļauts** programmatūrā Microsoft Defender Office 365 1. plānam, Office 365 Enterprise E3 un citiem Microsoft 365 programmas darbam abonementiem.</span><span class="sxs-lookup"><span data-stu-id="aba83-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1, Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="aba83-106">Kontam, kuru izmantojat simulētu uzbrukumu palaišanai, ir nepieciešamas globālā administratora vai drošības administratora atļaujas un daudzpakāpju autentifikācija (multi-factor authentication — MFA).</span><span class="sxs-lookup"><span data-stu-id="aba83-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="aba83-107">Papildinformāciju par uzbrukumu simulatora prasībām skatiet [šajā tēmā.](/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="aba83-107">For more information about Attack Simulator requirements, see [this topic](/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="aba83-108">Svarīgas lietas, kas jāzina **par Brute Force Password uzbrukumu** simulācijām:</span><span class="sxs-lookup"><span data-stu-id="aba83-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="aba83-109">Ja mērķa kontā ir iespējota MFA un parole tika uzminēta pareizi, konts netiks rādīts kā uz apdraudējuma (otrais autentifikācijas faktors būs nepilnīgs).</span><span class="sxs-lookup"><span data-stu-id="aba83-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="aba83-110">Paroles fails nedrīkst būt lielāks par 10 MB.</span><span class="sxs-lookup"><span data-stu-id="aba83-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="aba83-111">Izmantojiet vienu paroli katrā rindiņā un pēc pēdējās paroles sarakstā iekļaujiet tukšu rindiņu (rakstatgriezi).</span><span class="sxs-lookup"><span data-stu-id="aba83-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="aba83-112">Svarīgas lietas, kas jāzina par **Pikšķerēšanas attach** simulācijām:</span><span class="sxs-lookup"><span data-stu-id="aba83-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="aba83-113">Pikšķerēšanas pieteikšanās servera URL nevar norādīt pielāgotu **vērtību.**</span><span class="sxs-lookup"><span data-stu-id="aba83-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="aba83-114">Ja adresāts izmanto pievienojumprogrammu Iespējot atskaišu ziņojumu, lai ziņotu par [ziņojumu](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) kā pikšķerēšanas ziņojumu, iespējams, nesaņemsit brīdinājumus par ziņojumu (jo tas ir simulēts uzbrukums).</span><span class="sxs-lookup"><span data-stu-id="aba83-114">If a recipient uses the [Enable the Report Message add-in](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="aba83-115">Atskaites. Kad simulētais uzbrukums ir pabeigts, varat noklikšķināt uz Detalizēta informācija par **uzbrukumu,** lai skatītu atskaiti.</span><span class="sxs-lookup"><span data-stu-id="aba83-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="aba83-116">Detalizētus norādījumus un jaunos līdzekļus attack simulatorā skatiet rakstā [Attack Simulator in Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="aba83-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span></span>
