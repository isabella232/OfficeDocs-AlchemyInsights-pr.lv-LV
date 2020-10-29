---
title: Problēmu novēršana saistībā ar Microsoft Defender darbam ar Office 365 (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: cf54d5b3b854587202ff1b575889b9602228dd06
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801414"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="c0f74-102">Problēmu novēršana saistībā ar Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="c0f74-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="c0f74-103">Vai **pamanāt aizkaves ar e-pasta ziņojumu piegādi** ?</span><span class="sxs-lookup"><span data-stu-id="c0f74-103">**Notice delays with email message delivery** ?</span></span> <span data-ttu-id="c0f74-104">Izmēģiniet savas ATP drošas pielikumu politikas.</span><span class="sxs-lookup"><span data-stu-id="c0f74-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="c0f74-105">Tādējādi izvairīsities no e-pasta ziņojumu piegādes kavējumiem, aizsargājot adresātus no kaitīgiem failiem.</span><span class="sxs-lookup"><span data-stu-id="c0f74-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="c0f74-106">Vai **vēlaties ziņot par aplamiem pozitīviem vai aplamiem negatīviem** ?</span><span class="sxs-lookup"><span data-stu-id="c0f74-106">**Do you want to report false positives or false negatives** ?</span></span> <span data-ttu-id="c0f74-107">Izmantojiet šo saiti, lai iesniegtu failu analīzēm: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="c0f74-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="c0f74-108">**Vai zinājāt, ka varat IESPĒJOT ATP drošu saišu aizsardzību e-pastam, kas tiek sūtīts starp personām jūsu organizācijā** ?</span><span class="sxs-lookup"><span data-stu-id="c0f74-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization** ?</span></span> <span data-ttu-id="c0f74-109">Izpildiet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="c0f74-109">Follow these steps:</span></span>
    1. <span data-ttu-id="c0f74-110">Dodieties uz https://protection.office.com un pierakstieties.</span><span class="sxs-lookup"><span data-stu-id="c0f74-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="c0f74-111">Dodieties uz **draudu pārvaldības**  >  **politikas**  >  **drošās saites** .</span><span class="sxs-lookup"><span data-stu-id="c0f74-111">Go to **Threat management** > **Policy** > **Safe Links** .</span></span>
    3. <span data-ttu-id="c0f74-112">Sadaļā politikas **, kas attiecas uz konkrētiem adresātiem** , rediģējiet (vai pievienojiet) politiku.</span><span class="sxs-lookup"><span data-stu-id="c0f74-112">Under **Policies that apply to specific recipients** , edit (or add) a policy.</span></span>
    4. <span data-ttu-id="c0f74-113">Atlasiet **lietot drošas saites ziņojumiem** , kas nosūtīti uz organizāciju.</span><span class="sxs-lookup"><span data-stu-id="c0f74-113">Select **Apply safe links to messages sent within the organization** .</span></span>
    5. <span data-ttu-id="c0f74-114">Saglabājiet savu politiku un atvēliet aptuveni 30 minūtes, lai izmaiņas darbotos savā datu centrā.</span><span class="sxs-lookup"><span data-stu-id="c0f74-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="c0f74-115">Lai saņemtu papildu palīdzību par ATP, skatiet rakstu [Microsoft Defender darbam ar Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="c0f74-115">To get more help with ATP, see [Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>