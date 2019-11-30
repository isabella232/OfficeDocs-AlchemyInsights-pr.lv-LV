---
title: Labošana Office Apps Atvainojiet, mums ir pagaidu servera problēmas ziņojums
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
ms.openlocfilehash: 4b90f843843416408d7f3091325fe436dc3ec9df
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627997"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="cb87e-102">Office lietojumprogrammu labošana "Atvainojiet, mums ir pagaidu servera problēmas" ziņojums</span><span class="sxs-lookup"><span data-stu-id="cb87e-102">Fixing the Office apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="cb87e-103">Ja saņemat šo ziņojumu, mēģiniet veikt šādas darbības:</span><span class="sxs-lookup"><span data-stu-id="cb87e-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="cb87e-104">Pārbaudiet ugunsmūra, pretvīrusu programmatūras un starpniekservera iestatījumus, lai pārliecinātos, vai tie nebloķē interneta piekļuvi Office lietojumprogrammām.</span><span class="sxs-lookup"><span data-stu-id="cb87e-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="cb87e-105">Skatiet [Office 365 vietrāžus URL un IP adrešu diapazonus](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="cb87e-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="cb87e-106">Dodieties uz **Sākt** > **palaišanu**un pēc tam ierakstiet **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="cb87e-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="cb87e-107">Pārliecinieties, vai darbojas šādi pakalpojumi:</span><span class="sxs-lookup"><span data-stu-id="cb87e-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="cb87e-108">Tīklam pievienotās ierīces automātiskā iestatīšana</span><span class="sxs-lookup"><span data-stu-id="cb87e-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="cb87e-109">Tīkla saraksta pakalpojums</span><span class="sxs-lookup"><span data-stu-id="cb87e-109">Network List Service</span></span>
    - <span data-ttu-id="cb87e-110">Tīkla atrašanās vietas apzināšana</span><span class="sxs-lookup"><span data-stu-id="cb87e-110">Network Location Awareness</span></span>
    - <span data-ttu-id="cb87e-111">Windows notikumu žurnālā</span><span class="sxs-lookup"><span data-stu-id="cb87e-111">Windows Event Log</span></span>

<span data-ttu-id="cb87e-112">Ja kāds no šiem pakalpojumiem nedarbojas, mēģiniet to startēt.</span><span class="sxs-lookup"><span data-stu-id="cb87e-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="cb87e-113">Ja jums ir problēma, startējot pakalpojumu, izpildiet šādu komandu, atverot komandu uzvedni ar paaugstinātām atļaujām:</span><span class="sxs-lookup"><span data-stu-id="cb87e-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="cb87e-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="cb87e-114">**sfc /scannow**</span></span>

<span data-ttu-id="cb87e-115">Pēc tam, kad šī komanda ir pabeigta, restartējiet datoru.</span><span class="sxs-lookup"><span data-stu-id="cb87e-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="cb87e-116">Lai iegūtu detalizētu informāciju, skatiet sadaļu ["Atvainojiet, mēs nevaram izveidot savienojumu ar jūsu kontu. Lūdzu, vēlāk mēģiniet vēlreiz "kļūda, aktivizējot Office no Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="cb87e-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>