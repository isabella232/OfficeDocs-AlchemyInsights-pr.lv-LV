---
title: 2681 uzbrukuma simulators programmā Microsoft 365
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
ms.openlocfilehash: dec96238c8438dcf9df176e3e3f20bd8a985b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47759226"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="a8cb7-102">Uzbrukuma simulators programmā Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="a8cb7-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="a8cb7-103">Vai jums trūkst uzbrukuma simulators?</span><span class="sxs-lookup"><span data-stu-id="a8cb7-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="a8cb7-104">Uzbrukuma simulatoram ir nepieciešams **office 365 uzlabots draudu aizsardzības plāns 2 (ATP 2. plāns)** vai **Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="a8cb7-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="a8cb7-105">Uzbrukuma simulators **nav iekļauts** produktā Office 365 Advanced Threat Protection Plan 1 (ATP 1. plāns), Office 365 Enterprise E3 vai Microsoft 365 lietojumprogrammas darbam ar abonementu.</span><span class="sxs-lookup"><span data-stu-id="a8cb7-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="a8cb7-106">Kontam, ko izmantojat, lai palaistu simulētos uzbrukumus, nepieciešama globālā administratora vai drošības administratora atļaujas un daudzfaktoru autentifikācija (MFA).</span><span class="sxs-lookup"><span data-stu-id="a8cb7-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="a8cb7-107">Papildinformāciju par uzbrukuma simulatora prasībām skatiet [šajā tēmā](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="a8cb7-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="a8cb7-108">Svarīgas lietas, kas jāzina par **brutālas spēku paroļu** uzbrukuma simulācijām:</span><span class="sxs-lookup"><span data-stu-id="a8cb7-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="a8cb7-109">Ja adresāta kontam ir iespējota MFA un parole ir uzrakstīta pareizi, konts netiks rādīts kā kompromitēts (otrais autentifikācijas faktors nebūs pilnīgs).</span><span class="sxs-lookup"><span data-stu-id="a8cb7-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="a8cb7-110">Paroles fails nedrīkst būt lielāks par 10 MB.</span><span class="sxs-lookup"><span data-stu-id="a8cb7-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="a8cb7-111">Izmantojiet vienu paroli katrai rindiņai un pēc pēdējās saraksta paroles iekļaujiet tukšu rindiņu (rakstatgriezes).</span><span class="sxs-lookup"><span data-stu-id="a8cb7-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="a8cb7-112">Svarīgas lietas, kas jāzina par **šķēpa pikšķerēšanas** pievienošanu simulācijām:</span><span class="sxs-lookup"><span data-stu-id="a8cb7-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="a8cb7-113">Pēc noformējuma nevar nodrošināt pielāgotu vērtību **pikšķerēšanas pieteikšanās servera URL**.</span><span class="sxs-lookup"><span data-stu-id="a8cb7-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="a8cb7-114">Ja adresāts izmanto [Iespējot atskaites ziņojuma pievienojumprogrammu](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) , lai ziņotu par ziņojumu kā pikšķerēšanu, iespējams, nesaņemsit brīdinājumus par ziņojumu (jo tas ir simulēts uzbrukums).</span><span class="sxs-lookup"><span data-stu-id="a8cb7-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="a8cb7-115">Atskaites: kad Simulētais uzbrukums ir pabeigts, varat noklikšķināt uz **uzbrukt detalizēti** , lai skatītu atskaiti.</span><span class="sxs-lookup"><span data-stu-id="a8cb7-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="a8cb7-116">Detalizētus norādījumus un jaunus līdzekļus Attack simulatorā skatiet rakstā [Microsoft 365 uzbrukuma simulators](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="a8cb7-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
