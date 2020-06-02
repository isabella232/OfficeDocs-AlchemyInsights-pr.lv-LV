---
title: 2681 uzbrukums simulators Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 3dae4768ca62757ce7f92dfc527078c963d72742
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506745"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="a99c3-102">Uzbrukums simulators Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="a99c3-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="a99c3-103">Vai jums trūkst uzbrukums simulators?</span><span class="sxs-lookup"><span data-stu-id="a99c3-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="a99c3-104">Attack Simulator nepieciešama **office 365 uzlabotā Pretdraudu aizsardzības plāns 2 (ATP plāns 2)** vai **Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="a99c3-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="a99c3-105">Uzbrukuma simulators nav **iekļauts office** 365 uzlabotā Pretdraudu aizsardzības plānā 1 (ATP Plan 1), Office 365 Enterprise E3 vai jebkura Microsoft 365 programmas uzņēmumu abonementiem.</span><span class="sxs-lookup"><span data-stu-id="a99c3-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="a99c3-106">Kontu, ko izmanto, lai palaistu simulēta uzbrukumiem nepieciešama globālā administratora vai drošības administratora atļaujas un vairāku faktoru autentifikācija (MFA).</span><span class="sxs-lookup"><span data-stu-id="a99c3-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="a99c3-107">Lai iegūtu papildinformāciju par uzbrukuma simulatora prasībām, skatiet [šo tēmu](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="a99c3-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="a99c3-108">Svarīgas lietas, kas jāzina par **brutālu spēku parole** uzbrukums simulācijas:</span><span class="sxs-lookup"><span data-stu-id="a99c3-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="a99c3-109">Ja mērķa konts ir iespējots MFA un parole ir uzminējis pareizi, konts netiks rādīta kā apdraudēta (otrais autentifikācijas koeficients būs nepilnīga).</span><span class="sxs-lookup"><span data-stu-id="a99c3-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="a99c3-110">Paroles fails nevar būt lielāks par 10 MB.</span><span class="sxs-lookup"><span data-stu-id="a99c3-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="a99c3-111">Katrā rindiņā izmantojiet vienu paroli un iekļaujiet tukšu rindiņu (rakstatgrieze) pēc pēdējās paroles sarakstā.</span><span class="sxs-lookup"><span data-stu-id="a99c3-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="a99c3-112">Svarīgas lietas, kas jāzina par **šķēpu pikšķerēšana** pievienot simulācijas:</span><span class="sxs-lookup"><span data-stu-id="a99c3-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="a99c3-113">Pēc noformējuma nevar nodrošināt pielāgotu vērtību **pikšķerēšanas pieteikšanās servera URL**.</span><span class="sxs-lookup"><span data-stu-id="a99c3-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="a99c3-114">Ja adresāts izmanto atskaišu [ziņojumu pievienojumprogrammu iespējot](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) , lai ziņotu par ziņojumu kā pikšķerēšanu, iespējams, nesaņemsit ziņojuma brīdinājumus (jo tas ir simulēts uzbrukums).</span><span class="sxs-lookup"><span data-stu-id="a99c3-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="a99c3-115">Ziņojumi: pēc simulēta uzbrukums ir pabeigta, jūs varat noklikšķināt **uzbrukums detaļas** redzēt ziņojumu.</span><span class="sxs-lookup"><span data-stu-id="a99c3-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="a99c3-116">Detalizētus norādījumus un jaunas funkcijas uzbrukumu simulatorā skatiet [Attack Simulator Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="a99c3-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
