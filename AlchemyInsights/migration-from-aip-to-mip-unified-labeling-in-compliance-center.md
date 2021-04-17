---
title: Migrēšana no AIP uz MIP/vienotās etiķetes atbilstības centrā
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 12f5f5c46edd7918618c55a8a1905f3b28643092
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825378"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="4d342-102">Migrēšana no AIP uz MIP/vienotās etiķetes atbilstības centrā</span><span class="sxs-lookup"><span data-stu-id="4d342-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="4d342-103">Lai migrētu no AIP etiķetēm uz vienoto uzlīmēšanu drošības un atbilstības centrā, rīkojieties šādi:</span><span class="sxs-lookup"><span data-stu-id="4d342-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="4d342-104">**Aizsardzības aktivizēšana no Azure portāla**</span><span class="sxs-lookup"><span data-stu-id="4d342-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="4d342-105">Ja vēl neesat to izdarījis, atveriet jaunu pārlūkprogrammas logu [un pierakstieties Azure portālā.](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="4d342-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="4d342-106">Naviģējiet uz **Azure informācijas aizsardzības asmens stieņu.**</span><span class="sxs-lookup"><span data-stu-id="4d342-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="4d342-107">Piemēram, centrmezgla izvēlnē noklikšķiniet uz **Visi pakalpojumi** un sāciet **rakstīt informācija** lodziņā Filtrs.</span><span class="sxs-lookup"><span data-stu-id="4d342-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="4d342-108">Atlasiet **Azure informācijas aizsardzība**.</span><span class="sxs-lookup"><span data-stu-id="4d342-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="4d342-109">Ja iepriekš neesat piekļuvis Azure informācijas aizsardzības asmenim, skatiet vienreizējās papildu darbības, lai šo asmeni pievienotu portālam. [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time)</span><span class="sxs-lookup"><span data-stu-id="4d342-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="4d342-110">Lai atvērtu Azure informācijas aizsardzības asmens stieņu, ir nepieciešams [Azure Informācijas](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) aizsardzības Premium plāns vai Office 365 plāns, kurā ir iekļauta tiesību pārvaldība.</span><span class="sxs-lookup"><span data-stu-id="4d342-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="4d342-111">Ja jums ir kāds no šiem abonementiem, bet tiek parādīts ziņojums, ka nevar atrast derīgu abonementu, sazinieties ar [Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) atbalsta dienestu vai izmantojiet standarta atbalsta kanālus.</span><span class="sxs-lookup"><span data-stu-id="4d342-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="4d342-112">Atrodiet **izvēlnes opciju** Pārvaldība un atlasiet Aizsardzība **aktivizācija**.</span><span class="sxs-lookup"><span data-stu-id="4d342-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="4d342-113">Noklikšķiniet **uz** Aktivizēt un pēc tam apstipriniet savu darbību.</span><span class="sxs-lookup"><span data-stu-id="4d342-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="4d342-114">Kad aktivizācija ir pabeigta, informācijas joslā ir redzams, ka **aktivizēšana ir sekmīgi pabeigta.**</span><span class="sxs-lookup"><span data-stu-id="4d342-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="4d342-115">**Azure informācijas aizsardzības etiķešu migrēšana uz Office 365 & atbilstības centru**</span><span class="sxs-lookup"><span data-stu-id="4d342-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="4d342-116">Pārliecinieties, vai esat pieteicies kā lietotājs ar globālā administratora atļauju.</span><span class="sxs-lookup"><span data-stu-id="4d342-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="4d342-117">Naviģējiet uz **Azure informācijas aizsardzības asmens stieņu.**</span><span class="sxs-lookup"><span data-stu-id="4d342-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="4d342-118">Izvēlnes **opcijā** Pārvaldīt atlasiet **Vienotā etiķetēšana**.</span><span class="sxs-lookup"><span data-stu-id="4d342-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="4d342-119">Azure Informācijas **aizsardzības vietnē — vienotās uzlīmju asmensmens** nosaukums noklikšķiniet uz **Aktivizēt** un izpildiet tiešsaistes norādījumus.</span><span class="sxs-lookup"><span data-stu-id="4d342-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="4d342-120">**Piezīme.** Pārliecinieties, vai jums ir nepieciešamās atļaujas, pirms aktivizējot & atbilstības centra migrāciju.</span><span class="sxs-lookup"><span data-stu-id="4d342-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="4d342-121">Papildinformāciju skatiet šajos rakstos:</span><span class="sxs-lookup"><span data-stu-id="4d342-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="4d342-122">Vai jums ir jābūt globālajam administratoram, lai konfigurētu Azure informācijas aizsardzību, vai vai varu deleģēt citiem administratoriem?</span><span class="sxs-lookup"><span data-stu-id="4d342-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="4d342-123">Svarīga informācija par administratīvajām lomām pēc migrēšanas uz & atbilstības centru.</span><span class="sxs-lookup"><span data-stu-id="4d342-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="4d342-124">Papildinformāciju par AIP uz vienoto uzlīmju migrāciju uz drošības un atbilstības centru skatiet rakstā [Etiķešu migrēšana.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)</span><span class="sxs-lookup"><span data-stu-id="4d342-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
