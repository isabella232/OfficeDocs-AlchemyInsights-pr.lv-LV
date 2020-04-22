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
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716179"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="fb5ce-102">Office lietojumprogrammu labošana "mēs nevaram izveidot savienojumu tieši tagad" ziņojums</span><span class="sxs-lookup"><span data-stu-id="fb5ce-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="fb5ce-103">Ja saņemat šo ziņojumu, mēģiniet veikt šādas darbības:</span><span class="sxs-lookup"><span data-stu-id="fb5ce-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="fb5ce-104">Pārbaudiet ugunsmūra, pretvīrusu programmatūras un starpniekservera iestatījumus, lai pārliecinātos, vai tie nebloķē interneta piekļuvi Office lietojumprogrammām.</span><span class="sxs-lookup"><span data-stu-id="fb5ce-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="fb5ce-105">Skatiet [Microsoft URL un IP adrešu diapazoni](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="fb5ce-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="fb5ce-106">Dodieties uz **Sākt** > **palaišanu**un pēc tam ierakstiet **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="fb5ce-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="fb5ce-107">Pārliecinieties, vai darbojas šādi pakalpojumi:</span><span class="sxs-lookup"><span data-stu-id="fb5ce-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="fb5ce-108">Tīklam pievienotās ierīces automātiskā iestatīšana</span><span class="sxs-lookup"><span data-stu-id="fb5ce-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="fb5ce-109">Tīkla saraksta pakalpojums</span><span class="sxs-lookup"><span data-stu-id="fb5ce-109">Network List Service</span></span>
    - <span data-ttu-id="fb5ce-110">Tīkla atrašanās vietas apzināšana</span><span class="sxs-lookup"><span data-stu-id="fb5ce-110">Network Location Awareness</span></span>
    - <span data-ttu-id="fb5ce-111">Windows notikumu žurnālā</span><span class="sxs-lookup"><span data-stu-id="fb5ce-111">Windows Event Log</span></span>

<span data-ttu-id="fb5ce-112">Ja kāds no šiem pakalpojumiem nedarbojas, mēģiniet to startēt.</span><span class="sxs-lookup"><span data-stu-id="fb5ce-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="fb5ce-113">Ja jums ir problēma, startējot pakalpojumu, izpildiet šādu komandu, atverot komandu uzvedni ar paaugstinātām atļaujām:</span><span class="sxs-lookup"><span data-stu-id="fb5ce-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="fb5ce-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="fb5ce-114">**sfc /scannow**</span></span>

<span data-ttu-id="fb5ce-115">Pēc tam, kad šī komanda ir pabeigta, restartējiet datoru.</span><span class="sxs-lookup"><span data-stu-id="fb5ce-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="fb5ce-116">Lai iegūtu detalizētu informāciju, skatiet sadaļu ["Atvainojiet, mēs nevaram izveidot savienojumu ar jūsu kontu. Lūdzu, vēlāk mēģiniet vēlreiz "kļūda, aktivizējot Office no Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="fb5ce-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>