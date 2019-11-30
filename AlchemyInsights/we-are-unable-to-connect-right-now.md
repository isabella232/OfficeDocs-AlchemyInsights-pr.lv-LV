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
ms.openlocfilehash: 84e3a7700558ad8a5fad5b7ded6354fe8736e0f7
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628249"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="0ab84-102">Office lietojumprogrammu labošana "mēs nevaram izveidot savienojumu tieši tagad" ziņojums</span><span class="sxs-lookup"><span data-stu-id="0ab84-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="0ab84-103">Ja saņemat šo ziņojumu, mēģiniet veikt šādas darbības:</span><span class="sxs-lookup"><span data-stu-id="0ab84-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="0ab84-104">Pārbaudiet ugunsmūra, pretvīrusu programmatūras un starpniekservera iestatījumus, lai pārliecinātos, vai tie nebloķē interneta piekļuvi Office lietojumprogrammām.</span><span class="sxs-lookup"><span data-stu-id="0ab84-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="0ab84-105">Skatiet [Office 365 vietrāžus URL un IP adrešu diapazonus](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="0ab84-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="0ab84-106">Dodieties uz **Sākt** > **palaišanu**un pēc tam ierakstiet **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="0ab84-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="0ab84-107">Pārliecinieties, vai darbojas šādi pakalpojumi:</span><span class="sxs-lookup"><span data-stu-id="0ab84-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="0ab84-108">Tīklam pievienotās ierīces automātiskā iestatīšana</span><span class="sxs-lookup"><span data-stu-id="0ab84-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="0ab84-109">Tīkla saraksta pakalpojums</span><span class="sxs-lookup"><span data-stu-id="0ab84-109">Network List Service</span></span>
    - <span data-ttu-id="0ab84-110">Tīkla atrašanās vietas apzināšana</span><span class="sxs-lookup"><span data-stu-id="0ab84-110">Network Location Awareness</span></span>
    - <span data-ttu-id="0ab84-111">Windows notikumu žurnālā</span><span class="sxs-lookup"><span data-stu-id="0ab84-111">Windows Event Log</span></span>

<span data-ttu-id="0ab84-112">Ja kāds no šiem pakalpojumiem nedarbojas, mēģiniet to startēt.</span><span class="sxs-lookup"><span data-stu-id="0ab84-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="0ab84-113">Ja jums ir problēma, startējot pakalpojumu, izpildiet šādu komandu, atverot komandu uzvedni ar paaugstinātām atļaujām:</span><span class="sxs-lookup"><span data-stu-id="0ab84-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="0ab84-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="0ab84-114">**sfc /scannow**</span></span>

<span data-ttu-id="0ab84-115">Pēc tam, kad šī komanda ir pabeigta, restartējiet datoru.</span><span class="sxs-lookup"><span data-stu-id="0ab84-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="0ab84-116">Lai iegūtu detalizētu informāciju, skatiet sadaļu ["Atvainojiet, mēs nevaram izveidot savienojumu ar jūsu kontu. Lūdzu, vēlāk mēģiniet vēlreiz "kļūda, aktivizējot Office no Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="0ab84-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>