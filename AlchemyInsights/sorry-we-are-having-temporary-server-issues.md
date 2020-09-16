---
title: Microsoft 365 programmu labošana Diemžēl mums ir ziņojumi par pagaidu servera problēmām
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758252"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="583ee-102">Izlabojot Microsoft 365 lietojumprogrammas, tiek parādīts ziņojums "Diemžēl radās īslaicīgas problēmas ar serveri"</span><span class="sxs-lookup"><span data-stu-id="583ee-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="583ee-103">Ja tiek parādīts šis ziņojums, izmēģiniet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="583ee-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="583ee-104">Pārbaudiet savu ugunsmūri, pretvīrusu programmatūru un starpniekservera iestatījumus, lai pārliecinātos, vai tie nebloķē interneta piekļuvi Microsoft 365 programmām.</span><span class="sxs-lookup"><span data-stu-id="583ee-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="583ee-105">Skatiet [vietrāžus URL un IP adrešu diapazoni](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="583ee-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="583ee-106">Dodieties uz **Sākt**  >  **izpildi**un pēc tam ierakstiet **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="583ee-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="583ee-107">Pārliecinieties, vai visi šie pakalpojumi darbojas:</span><span class="sxs-lookup"><span data-stu-id="583ee-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="583ee-108">Tīkla pievienotās ierīces automātiskā iestatīšana</span><span class="sxs-lookup"><span data-stu-id="583ee-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="583ee-109">Tīkla saraksta pakalpojums</span><span class="sxs-lookup"><span data-stu-id="583ee-109">Network List Service</span></span>
    - <span data-ttu-id="583ee-110">Tīkla vietas izpratne</span><span class="sxs-lookup"><span data-stu-id="583ee-110">Network Location Awareness</span></span>
    - <span data-ttu-id="583ee-111">Windows notikumu žurnāls</span><span class="sxs-lookup"><span data-stu-id="583ee-111">Windows Event Log</span></span>

<span data-ttu-id="583ee-112">Ja kāds no šiem pakalpojumiem nedarbojas, mēģiniet sākt to.</span><span class="sxs-lookup"><span data-stu-id="583ee-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="583ee-113">Ja rodas problēmas, sākot pakalpojumu, izpildiet šādu komandu, atverot komandu uzvedni ar paaugstinātām atļaujām:</span><span class="sxs-lookup"><span data-stu-id="583ee-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="583ee-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="583ee-114">**sfc /scannow**</span></span>

<span data-ttu-id="583ee-115">Kad šī komanda ir pabeigta, restartējiet datoru.</span><span class="sxs-lookup"><span data-stu-id="583ee-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="583ee-116">Detalizētu informāciju skatiet rakstā ["Diemžēl mēs nevaram izveidot savienojumu ar jūsu kontu. Lūdzu, mēģiniet vēlreiz vēlāk, kad aktivizējat](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="583ee-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>