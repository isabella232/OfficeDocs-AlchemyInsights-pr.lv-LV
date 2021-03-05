---
title: Problēma ar AAD Connect darbspējas
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482070"
---
# <a name="problem-with-aad-connect-health"></a><span data-ttu-id="9653f-102">Problēma ar AAD Connect darbspējas</span><span class="sxs-lookup"><span data-stu-id="9653f-102">Problem with AAD Connect Health</span></span>

- <span data-ttu-id="9653f-103">Pārliecinieties, vai jums ir atļauts veikt šo darbību.</span><span class="sxs-lookup"><span data-stu-id="9653f-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="9653f-104">Globālajiem administratoriem pēc noklusējuma ir piekļuve.</span><span class="sxs-lookup"><span data-stu-id="9653f-104">Global Admins have access by default.</span></span> <span data-ttu-id="9653f-105">Turklāt varat izmantot [lomai bāzētu piekļuves vadību](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) , lai deleģētu reģistrācijas atļaujas līdzstrādniekiem.</span><span class="sxs-lookup"><span data-stu-id="9653f-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="9653f-106">Pārliecinieties, vai nepieciešamie galapunkti ir iespējoti, bet nav bloķēti ugunsmūra dēļ.</span><span class="sxs-lookup"><span data-stu-id="9653f-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="9653f-107">Detalizētu informāciju skatiet sadaļā [prasības](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span><span class="sxs-lookup"><span data-stu-id="9653f-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="9653f-108">Reģistrācija var neizdoties, jo izejošā komunikācija tiek pakļauta SSL pārbaudei tīkla slānī.</span><span class="sxs-lookup"><span data-stu-id="9653f-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="9653f-109">Pārliecinieties, vai esat pārbaudījis Azure AD Connect darbspējas paziņojumu iestatījumus.</span><span class="sxs-lookup"><span data-stu-id="9653f-109">Make sure you have verified the notification settings for Azure AD Connect Health.</span></span> <span data-ttu-id="9653f-110">Lūdzu, pārskatiet savu iestatījumu.</span><span class="sxs-lookup"><span data-stu-id="9653f-110">Please review your setting.</span></span> <span data-ttu-id="9653f-111">Šajā [rokasgrāmatā](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) varat palīdzēt saprast, kā konfigurēt Azure AD Connect paziņojumi par paziņojumu iestatījumiem.</span><span class="sxs-lookup"><span data-stu-id="9653f-111">This [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) can help you understand how to configure the notification settings for Azure AD Connect health notifications.</span></span>
- <span data-ttu-id="9653f-112">Lai uzzinātu vairāk par to, kā AAD Connect Health sinhronizācijas atskaiti un kā to lejupielādēt, skatiet rakstu [objekta līmeņa sinhronizācijas atskaite](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span><span class="sxs-lookup"><span data-stu-id="9653f-112">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="9653f-113">Lai novērstu AAD savienojumu ar veselību brīdinājumus, izpildiet [norādījumus par to, kā AAD savienos](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) un bieži uzdotos jautājumus skatiet rakstā [bieži sastopamas AAD savienojuma](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)problēmas.</span><span class="sxs-lookup"><span data-stu-id="9653f-113">To troubleshoot AAD Connect Health alerts, follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
