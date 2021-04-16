---
title: Aktivizācijas problēma — pašlaik nevar izveidot savienojumu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 2dd3c97bb85254215b13ee8a1222941c0492b204
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806449"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="becbf-102">Microsoft 365 programmu kļūdas ziņojums "Šobrīd nevar izveidot savienojumu"</span><span class="sxs-lookup"><span data-stu-id="becbf-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="becbf-103">Ja saņemat šādu ziņojumu, mēģiniet veikt šādas darbības:</span><span class="sxs-lookup"><span data-stu-id="becbf-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="becbf-104">Pārbaudiet savu ugunsmūri, pretvīrusu programmatūru un starpniekservera iestatījumus, lai pārliecinātos, vai nebloķē piekļuvi internetam Microsoft 365 programmām.</span><span class="sxs-lookup"><span data-stu-id="becbf-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="becbf-105">Skatiet [rakstu Microsoft URL un IP adrešu diapazoni.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="becbf-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="becbf-106">Dodieties **uz Start**  >  **Run** un pēc tam ierakstiet **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="becbf-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="becbf-107">Pārliecinieties, vai darbojas tālāk sniegtie pakalpojumi.</span><span class="sxs-lookup"><span data-stu-id="becbf-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="becbf-108">Tīkla savienoto ierīču automātiskā iestatīšana</span><span class="sxs-lookup"><span data-stu-id="becbf-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="becbf-109">Tīkla saraksta pakalpojums</span><span class="sxs-lookup"><span data-stu-id="becbf-109">Network List Service</span></span>
    - <span data-ttu-id="becbf-110">Tīkla atrašanās vietas informētība</span><span class="sxs-lookup"><span data-stu-id="becbf-110">Network Location Awareness</span></span>
    - <span data-ttu-id="becbf-111">Windows notikumu žurnāls</span><span class="sxs-lookup"><span data-stu-id="becbf-111">Windows Event Log</span></span>

<span data-ttu-id="becbf-112">Ja kāds no šiem pakalpojumiem nedarbojas, mēģiniet to startēt.</span><span class="sxs-lookup"><span data-stu-id="becbf-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="becbf-113">Ja rodas problēma, startējot pakalpojumu, palaidiet tālāk norādīto komandu, atverot komandu uzvedni ar paaugstinātām atļaujām:</span><span class="sxs-lookup"><span data-stu-id="becbf-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="becbf-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="becbf-114">**sfc /scannow**</span></span>

<span data-ttu-id="becbf-115">Kad šī komanda ir pabeigta, restartējiet datoru.</span><span class="sxs-lookup"><span data-stu-id="becbf-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="becbf-116">Detalizētu informāciju skatiet sadaļā ["Diemžēl nevaram izveidot savienojumu ar jūsu kontu. Lūdzu, vēlāk mēģiniet vēlreiz", aktivizējot Office no Microsoft 365.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span><span class="sxs-lookup"><span data-stu-id="becbf-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>