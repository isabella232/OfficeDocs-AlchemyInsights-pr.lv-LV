---
title: Migrēšana no AIP uz MIP/vienotās marķēšanas atbilstības centrā
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674333"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="d4d52-102">Migrēšana no AIP uz MIP/vienotās marķēšanas atbilstības centrā</span><span class="sxs-lookup"><span data-stu-id="d4d52-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="d4d52-103">Lai migrētu no AIP etiķetēm uz vienotu marķējumu drošības un atbilstības centrā, rīkojieties šādi:</span><span class="sxs-lookup"><span data-stu-id="d4d52-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="d4d52-104">**Aizsardzības aktivizēšana no Azure portāla**</span><span class="sxs-lookup"><span data-stu-id="d4d52-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="d4d52-105">Ja vēl neesat to izdarījis, atveriet jaunu pārlūkprogrammas logu un [pierakstieties Azure portālā](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="d4d52-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="d4d52-106">Pārejiet uz **Azure informācijas aizsardzības** asmeni.</span><span class="sxs-lookup"><span data-stu-id="d4d52-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="d4d52-107">Piemēram, izvēlnē centrmezgls noklikšķiniet uz **Visi pakalpojumi** un sāciet rakstīt **informāciju** filtra lodziņā.</span><span class="sxs-lookup"><span data-stu-id="d4d52-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="d4d52-108">Atlasiet **Azure informācijas aizsardzība**.</span><span class="sxs-lookup"><span data-stu-id="d4d52-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="d4d52-109">Ja iepriekš neesat piekļuvis Azure informācijas aizsardzības diskam, skatiet vienreizējās [papildu darbības](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) , lai šo disku pievienotu portālam.</span><span class="sxs-lookup"><span data-stu-id="d4d52-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="d4d52-110">Lai atvērtu Azure Information Protection asmeni, jums ir jābūt [Azure Information Protection Premium plānam](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) vai Office 365 plānam, kurā ir iekļauta tiesību pārvaldība.</span><span class="sxs-lookup"><span data-stu-id="d4d52-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="d4d52-111">Ja jums ir kāds no šiem abonementiem, bet redzat ziņojumu, ka derīgu abonementu nevar atrast, [sazinieties ar Microsoft atbalsta dienestu](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) vai izmantojiet savus standarta atbalsta kanālus.</span><span class="sxs-lookup"><span data-stu-id="d4d52-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="d4d52-112">Atrodiet **pārvaldības** izvēlnes opcijas un atlasiet **aizsardzības aktivizēšana**.</span><span class="sxs-lookup"><span data-stu-id="d4d52-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="d4d52-113">Noklikšķiniet uz **Aktivizēt**un pēc tam apstipriniet savu darbību.</span><span class="sxs-lookup"><span data-stu-id="d4d52-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="d4d52-114">Kad aktivizēšana ir pabeigta, informācijas joslā aktivizācija ir **sekmīgi pabeigta**.</span><span class="sxs-lookup"><span data-stu-id="d4d52-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="d4d52-115">**Azure informācijas aizsardzības etiķešu migrēšana uz Office 365 drošības & atbilstības centrs**</span><span class="sxs-lookup"><span data-stu-id="d4d52-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="d4d52-116">Pārliecinieties, vai esat pieteicies kā lietotājs, kuram ir globālās administratora atļaujas.</span><span class="sxs-lookup"><span data-stu-id="d4d52-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="d4d52-117">Pārejiet uz **Azure informācijas aizsardzības** asmeni.</span><span class="sxs-lookup"><span data-stu-id="d4d52-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="d4d52-118">Izvēlnē **Manage (pārvaldīt** ) atlasiet **vienota marķēšana**.</span><span class="sxs-lookup"><span data-stu-id="d4d52-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="d4d52-119">**Azure Information Protection — vienotās marķēšanas** asmens, noklikšķiniet uz **Aktivizēt** un izpildiet tiešsaistes instrukcijas.</span><span class="sxs-lookup"><span data-stu-id="d4d52-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="d4d52-120">**Piezīme**. Pārbaudiet, vai jums ir atbilstošas atļaujas, pirms aktivizējat drošības & atbilstības centra migrāciju.</span><span class="sxs-lookup"><span data-stu-id="d4d52-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="d4d52-121">Lai iegūtu papildinformāciju, skatiet šos rakstus:</span><span class="sxs-lookup"><span data-stu-id="d4d52-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="d4d52-122">Vai jums ir jābūt globālajam administratoram, lai konfigurētu Azure informācijas aizsardzību vai varu deleģēt citiem administratoriem?</span><span class="sxs-lookup"><span data-stu-id="d4d52-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="d4d52-123">Svarīga informācija par administratīvajām lomām pēc migrēšanas uz drošības & atbilstības centru.</span><span class="sxs-lookup"><span data-stu-id="d4d52-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="d4d52-124">Lai iegūtu papildinformāciju par to, kā AIP ir vienots pārzīmju migrēšanas uz drošības un atbilstības centru, skatiet rakstu [etiķešu migrēšana](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="d4d52-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
