---
title: Nevar pieteikties programmā Teams, jo radās kļūda autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932039"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a><span data-ttu-id="98598-102">Nevar pieteikties programmā Teams, jo radās kļūda autologon.microsoftazuread-sso dot com:443</span><span class="sxs-lookup"><span data-stu-id="98598-102">Unable to log into Teams due to error autologon.microsoftazuread-sso dot com:443</span></span>

<span data-ttu-id="98598-103">Ja Seamless SSO ir iespējots kā O365 autentifikācija, iespējams, ka iekštīkla vietnēm jāpievieno URL “autologon.microsoftazuread-sso.com”.</span><span class="sxs-lookup"><span data-stu-id="98598-103">If Seamless SSO is enabled as the O365 authentication, the URL "autologon.microsoftazuread-sso.com" may need to be added to Intranet Sites.</span></span>  <span data-ttu-id="98598-104">Ja tas iepriekš ir pievienots uzticamajām vietnēm un tiek lietots Seamless SSO, tas ir jānoņem no uzticamajām vietnēm.</span><span class="sxs-lookup"><span data-stu-id="98598-104">If it has previously been added to Trusted Sites  and Seamless SSO is in use, it should be removed from Trusted Sites.</span></span>

<span data-ttu-id="98598-105">Lūdzu, pārskatiet [Seamless SSO problēmu novēršanas kontrolsarakstu](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span><span class="sxs-lookup"><span data-stu-id="98598-105">Please review the [Seamless SSO Troubleshooting Checklist](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span></span>

<span data-ttu-id="98598-106">Veiciet tālāk norādītās darbības, lai pievienotu URL iekštīkla vietņu sarakstam.</span><span class="sxs-lookup"><span data-stu-id="98598-106">Follow these steps to add a URL to Intranet Sites list:</span></span>

1. <span data-ttu-id="98598-107">Atveriet pārlūkprogrammu Internet Explorer, noklikšķinot uz pogas **Sākt**.</span><span class="sxs-lookup"><span data-stu-id="98598-107">Open Internet Explorer by clicking the **Start** button.</span></span> <span data-ttu-id="98598-108">Meklēšanas lodziņā ierakstiet Internet Explorer un pēc tam rezultātu sarakstā noklikšķiniet uz **Internet Explorer**.</span><span class="sxs-lookup"><span data-stu-id="98598-108">In the search box, type Internet Explorer, and then, in the list of results, click **Internet Explorer**.</span></span>
2. <span data-ttu-id="98598-109">Noklikšķiniet uz **Rīki** un pēc tam noklikšķiniet uz **Interneta opcijas**.</span><span class="sxs-lookup"><span data-stu-id="98598-109">Click **Tools**, and then click **Internet options**.</span></span>
3. <span data-ttu-id="98598-110">Noklikšķiniet uz cilnes **Drošība**.</span><span class="sxs-lookup"><span data-stu-id="98598-110">Click the **Security** tab.</span></span>
4. <span data-ttu-id="98598-111">Tagad noklikšķiniet uz **Lokālā iekštīkla vietnes** un pēc tam noklikšķiniet uz pogas **Vietnes** un pēc tam uz pogas **Papildu**.</span><span class="sxs-lookup"><span data-stu-id="98598-111">Now click on **Local Intranet sites** and then click on the **sites** button and then **Advanced** button.</span></span>
5. <span data-ttu-id="98598-112">Ievadiet tīmekļa vietnes URL un noklikšķiniet uz **Pievienot**.</span><span class="sxs-lookup"><span data-stu-id="98598-112">Enter the Website URL and click **Add**.</span></span>
6. <span data-ttu-id="98598-113">Kad esat pabeidzis, noklikšķiniet uz **Saglabāt**.</span><span class="sxs-lookup"><span data-stu-id="98598-113">When you are finished, click **Close**.</span></span>

<span data-ttu-id="98598-114">Papildinformāciju skatiet rakstā [Dokumentācija Seamless SSO izvietošanai pakalpojumā O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (3. darbībā ietverts uz politiku balstīts process URL pievienošanai iekštīkla vietnēs).</span><span class="sxs-lookup"><span data-stu-id="98598-114">For more information, see [Documentation for deploying Seamless SSO for O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (includes Policy-based process to add a URL to Intranet Sites in Step 3).</span></span>
