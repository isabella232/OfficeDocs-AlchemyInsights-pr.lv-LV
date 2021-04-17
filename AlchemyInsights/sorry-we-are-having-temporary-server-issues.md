---
title: Microsoft 365 programmu labošana Diemžēl mums ir īslaicīgu servera problēmu ziņojums
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
- "3420"
- "9001430"
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835278"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="7d9a5-102">Microsoft 365 lietojumprogrammu kļūdas ziņojums "Diemžēl mums ir īslaicīgas servera problēmas"</span><span class="sxs-lookup"><span data-stu-id="7d9a5-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="7d9a5-103">Ja saņemat šādu ziņojumu, mēģiniet veikt šādas darbības:</span><span class="sxs-lookup"><span data-stu-id="7d9a5-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="7d9a5-104">Pārbaudiet savu ugunsmūri, pretvīrusu programmatūru un starpniekservera iestatījumus, lai pārliecinātos, vai nebloķē piekļuvi internetam Microsoft 365 programmām.</span><span class="sxs-lookup"><span data-stu-id="7d9a5-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="7d9a5-105">Skatiet [rakstu URL un IP adrešu diapazoni.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="7d9a5-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="7d9a5-106">Dodieties **uz Start**  >  **Run** un pēc tam ierakstiet **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="7d9a5-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="7d9a5-107">Pārliecinieties, vai darbojas tālāk sniegtie pakalpojumi.</span><span class="sxs-lookup"><span data-stu-id="7d9a5-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="7d9a5-108">Tīkla savienoto ierīču automātiskā iestatīšana</span><span class="sxs-lookup"><span data-stu-id="7d9a5-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="7d9a5-109">Tīkla saraksta pakalpojums</span><span class="sxs-lookup"><span data-stu-id="7d9a5-109">Network List Service</span></span>
    - <span data-ttu-id="7d9a5-110">Tīkla atrašanās vietas informētība</span><span class="sxs-lookup"><span data-stu-id="7d9a5-110">Network Location Awareness</span></span>
    - <span data-ttu-id="7d9a5-111">Windows notikumu žurnāls</span><span class="sxs-lookup"><span data-stu-id="7d9a5-111">Windows Event Log</span></span>

<span data-ttu-id="7d9a5-112">Ja kāds no šiem pakalpojumiem nedarbojas, mēģiniet to startēt.</span><span class="sxs-lookup"><span data-stu-id="7d9a5-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="7d9a5-113">Ja rodas problēma, startējot pakalpojumu, palaidiet tālāk norādīto komandu, atverot komandu uzvedni ar paaugstinātām atļaujām:</span><span class="sxs-lookup"><span data-stu-id="7d9a5-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="7d9a5-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="7d9a5-114">**sfc /scannow**</span></span>

<span data-ttu-id="7d9a5-115">Kad šī komanda ir pabeigta, restartējiet datoru.</span><span class="sxs-lookup"><span data-stu-id="7d9a5-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="7d9a5-116">Detalizētu informāciju skatiet sadaļā ["Diemžēl nevaram izveidot savienojumu ar jūsu kontu. Lūdzu, vēlāk mēģiniet vēlreiz", kad aktivizējat.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span><span class="sxs-lookup"><span data-stu-id="7d9a5-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>