---
title: Problēmu novēršana saistībā ar Office 365 uzlabotā Pretdraudu aizsardzība (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 99bc985f2d66693aca45f0833ab47c043acc1324
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766752"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="4a50f-102">Office 365 ATP problēmu novēršana</span><span class="sxs-lookup"><span data-stu-id="4a50f-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="4a50f-103">**Pamanāt aizkavēšanos ar e-pasta ziņojumu piegādi**?</span><span class="sxs-lookup"><span data-stu-id="4a50f-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="4a50f-104">Mēģiniet izmantot jūsu ATP drošas pielikumu politikām dinamisko piegādes opciju.</span><span class="sxs-lookup"><span data-stu-id="4a50f-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="4a50f-105">Tas ļaus izvairīties no e-pasta ziņojumu piegādes kavējumiem, aizsargājot adresātus no ļaunprātīgiem failiem.</span><span class="sxs-lookup"><span data-stu-id="4a50f-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="4a50f-106">Vai **vēlaties ziņot par viltus pozitīviem vai viltus negatīviem**?</span><span class="sxs-lookup"><span data-stu-id="4a50f-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="4a50f-107">Izmantojiet šo saiti, lai iesniegtu failu analīzei:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="4a50f-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="4a50f-108">**Vai jūs zinājāt, ka jūs varat IESPĒJOT ATP drošas saites aizsardzību e-pastam, kas tiek sūtīts starp cilvēkiem jūsu organizācijā**?</span><span class="sxs-lookup"><span data-stu-id="4a50f-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="4a50f-109">Izpildiet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="4a50f-109">Follow these steps:</span></span>
    1. <span data-ttu-id="4a50f-110">Doties https://protection.office.com, un pierakstieties.</span><span class="sxs-lookup"><span data-stu-id="4a50f-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="4a50f-111">Pārejiet uz sadaļu **draudu pārvaldības** > **politika** > **drošas saites**.</span><span class="sxs-lookup"><span data-stu-id="4a50f-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="4a50f-112">Sadaļā **politikas, kas attiecas uz noteiktiem adresātiem**, rediģējiet (vai pievienojiet) politiku.</span><span class="sxs-lookup"><span data-stu-id="4a50f-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="4a50f-113">Atlasiet **lietot drošas saites uz ziņojumiem, kas tiek sūtīti organizācijas ietvaros**.</span><span class="sxs-lookup"><span data-stu-id="4a50f-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="4a50f-114">Saglabājiet politiku un atļaujiet aptuveni 30 minūtes, lai izmaiņas darbotos savā datu centrā.</span><span class="sxs-lookup"><span data-stu-id="4a50f-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="4a50f-115">Lai iegūtu papildu palīdzību par ATP, skatiet [Office 365 uzlabotā Pretdraudu aizsardzība](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="4a50f-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).</span></span>