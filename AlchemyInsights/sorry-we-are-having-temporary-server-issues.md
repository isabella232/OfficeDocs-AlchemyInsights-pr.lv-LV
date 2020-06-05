---
title: Labošana Microsoft 365 Apps Atvainojiet, mums ir pagaidu servera problēmas ziņojums
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582710"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="e7224-102">Fixing Microsoft 365 progr "Atvainojiet, mums ir pagaidu servera problēmas" ziņojums</span><span class="sxs-lookup"><span data-stu-id="e7224-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="e7224-103">Ja saņemat šo ziņojumu, mēģiniet veikt šādas darbības:</span><span class="sxs-lookup"><span data-stu-id="e7224-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="e7224-104">Pārbaudiet ugunsmūra, pretvīrusu programmatūras un starpniekservera iestatījumus, lai pārliecinātos, vai tie nebloķē interneta piekļuvi Microsoft 365 lietojumprogrammām.</span><span class="sxs-lookup"><span data-stu-id="e7224-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="e7224-105">Skatiet [vietrāžus URL un IP adrešu diapazonus](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="e7224-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="e7224-106">Dodieties uz **Sākt**  >  **palaišanu**un pēc tam ierakstiet **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="e7224-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="e7224-107">Pārliecinieties, vai darbojas šādi pakalpojumi:</span><span class="sxs-lookup"><span data-stu-id="e7224-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="e7224-108">Tīklam pievienotās ierīces automātiskā iestatīšana</span><span class="sxs-lookup"><span data-stu-id="e7224-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="e7224-109">Tīkla saraksta pakalpojums</span><span class="sxs-lookup"><span data-stu-id="e7224-109">Network List Service</span></span>
    - <span data-ttu-id="e7224-110">Tīkla atrašanās vietas apzināšana</span><span class="sxs-lookup"><span data-stu-id="e7224-110">Network Location Awareness</span></span>
    - <span data-ttu-id="e7224-111">Windows notikumu žurnālā</span><span class="sxs-lookup"><span data-stu-id="e7224-111">Windows Event Log</span></span>

<span data-ttu-id="e7224-112">Ja kāds no šiem pakalpojumiem nedarbojas, mēģiniet to startēt.</span><span class="sxs-lookup"><span data-stu-id="e7224-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="e7224-113">Ja jums ir problēma, startējot pakalpojumu, izpildiet šādu komandu, atverot komandu uzvedni ar paaugstinātām atļaujām:</span><span class="sxs-lookup"><span data-stu-id="e7224-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="e7224-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="e7224-114">**sfc /scannow**</span></span>

<span data-ttu-id="e7224-115">Pēc tam, kad šī komanda ir pabeigta, restartējiet datoru.</span><span class="sxs-lookup"><span data-stu-id="e7224-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="e7224-116">Lai iegūtu detalizētu informāciju, skatiet sadaļu ["Atvainojiet, mēs nevaram izveidot savienojumu ar jūsu kontu. Lūdzu, vēlāk mēģiniet vēlreiz "kļūda, aktivizējot](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="e7224-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>