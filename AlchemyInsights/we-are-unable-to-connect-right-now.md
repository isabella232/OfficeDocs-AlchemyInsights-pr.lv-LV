---
title: Aktivizācijas problēma-mēs nevaram izveidot savienojumu tieši tagad
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: b46bac60633ad9a006b9446919b8c99e221b07e4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581882"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="b3eff-102">Fixing Microsoft 365 progr "mēs nevaram izveidot savienojumu tieši tagad" ziņojums</span><span class="sxs-lookup"><span data-stu-id="b3eff-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="b3eff-103">Ja saņemat šo ziņojumu, mēģiniet veikt šādas darbības:</span><span class="sxs-lookup"><span data-stu-id="b3eff-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="b3eff-104">Pārbaudiet ugunsmūra, pretvīrusu programmatūras un starpniekservera iestatījumus, lai pārliecinātos, vai tie nebloķē interneta piekļuvi Microsoft 365 lietojumprogrammām.</span><span class="sxs-lookup"><span data-stu-id="b3eff-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="b3eff-105">Skatiet [Microsoft URL un IP adrešu diapazoni](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="b3eff-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="b3eff-106">Dodieties uz **Sākt**  >  **palaišanu**un pēc tam ierakstiet **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="b3eff-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="b3eff-107">Pārliecinieties, vai darbojas šādi pakalpojumi:</span><span class="sxs-lookup"><span data-stu-id="b3eff-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="b3eff-108">Tīklam pievienotās ierīces automātiskā iestatīšana</span><span class="sxs-lookup"><span data-stu-id="b3eff-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="b3eff-109">Tīkla saraksta pakalpojums</span><span class="sxs-lookup"><span data-stu-id="b3eff-109">Network List Service</span></span>
    - <span data-ttu-id="b3eff-110">Tīkla atrašanās vietas apzināšana</span><span class="sxs-lookup"><span data-stu-id="b3eff-110">Network Location Awareness</span></span>
    - <span data-ttu-id="b3eff-111">Windows notikumu žurnālā</span><span class="sxs-lookup"><span data-stu-id="b3eff-111">Windows Event Log</span></span>

<span data-ttu-id="b3eff-112">Ja kāds no šiem pakalpojumiem nedarbojas, mēģiniet to startēt.</span><span class="sxs-lookup"><span data-stu-id="b3eff-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="b3eff-113">Ja jums ir problēma, startējot pakalpojumu, izpildiet šādu komandu, atverot komandu uzvedni ar paaugstinātām atļaujām:</span><span class="sxs-lookup"><span data-stu-id="b3eff-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="b3eff-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="b3eff-114">**sfc /scannow**</span></span>

<span data-ttu-id="b3eff-115">Pēc tam, kad šī komanda ir pabeigta, restartējiet datoru.</span><span class="sxs-lookup"><span data-stu-id="b3eff-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="b3eff-116">Lai iegūtu detalizētu informāciju, skatiet sadaļu ["Atvainojiet, mēs nevaram izveidot savienojumu ar jūsu kontu. Lūdzu, vēlāk mēģiniet vēlreiz "kļūda, aktivizējot Office no Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="b3eff-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>