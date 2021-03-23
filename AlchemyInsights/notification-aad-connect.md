---
title: Brīdinājums AAD Connect
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036108"
---
# <a name="notification-aad-connect"></a><span data-ttu-id="51b51-102">Brīdinājums AAD Connect</span><span class="sxs-lookup"><span data-stu-id="51b51-102">Notification AAD Connect</span></span>

- <span data-ttu-id="51b51-103">Pārliecinieties, vai jums ir atļauts veikt šo darbību.</span><span class="sxs-lookup"><span data-stu-id="51b51-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="51b51-104">Globālajiem administratoriem pēc noklusējuma ir piekļuve.</span><span class="sxs-lookup"><span data-stu-id="51b51-104">Global Admins have access by default.</span></span> <span data-ttu-id="51b51-105">Turklāt varat izmantot [lomai bāzētu piekļuves vadību](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) , lai deleģētu reģistrācijas atļaujas līdzstrādniekiem.</span><span class="sxs-lookup"><span data-stu-id="51b51-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="51b51-106">Pārliecinieties, vai nepieciešamie galapunkti ir iespējoti, bet nav bloķēti ugunsmūra dēļ.</span><span class="sxs-lookup"><span data-stu-id="51b51-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="51b51-107">Detalizētu informāciju skatiet sadaļā [prasības](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span><span class="sxs-lookup"><span data-stu-id="51b51-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="51b51-108">Reģistrācija var neizdoties, jo izejošā komunikācija tiek pakļauta SSL pārbaudei tīkla slānī.</span><span class="sxs-lookup"><span data-stu-id="51b51-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="51b51-109">Pārliecinieties, vai esat pārbaudījis Azure AD Connect Health paziņojumu iestatījumus un pārskatiet savu iestatījumu.</span><span class="sxs-lookup"><span data-stu-id="51b51-109">Make sure you have verified the notification settings for Azure AD Connect Health and review your setting.</span></span> <span data-ttu-id="51b51-110">Lai uzzinātu, kā konfigurēt paziņojumu iestatījumus Azure AD Connect Health paziņojumiem, skatiet šo [rokasgrāmatu](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span><span class="sxs-lookup"><span data-stu-id="51b51-110">To understand how to configure the notification settings for Azure AD Connect Health notifications, see this [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span></span>
- <span data-ttu-id="51b51-111">Lai uzzinātu vairāk par to, kā AAD Connect Health sinhronizācijas atskaiti un kā to lejupielādēt, skatiet rakstu [objekta līmeņa sinhronizācijas atskaite](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span><span class="sxs-lookup"><span data-stu-id="51b51-111">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="51b51-112">Lai novērstu AAD savienojuma [ar veselību brīdinājumu](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)izpildi, skatiet [problēmu novēršanas norādījumus attiecībā uz AAD](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) .</span><span class="sxs-lookup"><span data-stu-id="51b51-112">To troubleshoot AAD Connect Health Alerts follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
