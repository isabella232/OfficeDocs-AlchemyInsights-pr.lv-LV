---
title: Problēmu novēršana programmatūrā Microsoft Defender Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 91d73853d3ea67d6c6954fffb32dd1428e3d9976
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545275"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="22335-102">Problēmu novēršana programmatūrā Microsoft Defender Office 365</span><span class="sxs-lookup"><span data-stu-id="22335-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="22335-103">**Vai pamanāt ziņojumu piegādes kavējumus?**</span><span class="sxs-lookup"><span data-stu-id="22335-103">**Do you notice delays in message delivery?**</span></span> <span data-ttu-id="22335-104">Izmantojiet opciju [Dinamiskā piegāde](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) savā programmatūrā Microsoft Defender Office 365 Seifs pielikumu politiku.</span><span class="sxs-lookup"><span data-stu-id="22335-104">Use the [Dynamic Delivery](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your Microsoft Defender for Office 365 Safe Attachments policy.</span></span> <span data-ttu-id="22335-105">Tas palīdzēs izvairīties no ziņojumu aizkaves, vienlaikus aizsargājot adresātus no ļaunprātīgiem failiem.</span><span class="sxs-lookup"><span data-stu-id="22335-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="22335-106">**Vai vēlaties ziņot Microsoft par aplami pozitīvajiem vai aplami negatīvajiem?**</span><span class="sxs-lookup"><span data-stu-id="22335-106">**Do you want to report false positives or false negatives to Microsoft?**</span></span> <span data-ttu-id="22335-107">Izmantojiet [submissions Explorer](https://protection.office.com/reportsubmission).</span><span class="sxs-lookup"><span data-stu-id="22335-107">Use [Submissions Explorer](https://protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="22335-108">-\*\* Vai zinājāt, ka varat iespējot iekšējo Seifs, kas tiek sūtīts starp adresātiem jūsu organizācijā, saišu aizsardzību?\*\* Veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="22335-108">-\*\* Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?\*\* Follow these steps:</span></span>

  1. <span data-ttu-id="22335-109">Dodieties [https://protection.office.com](https://protection.office.com) uz sadaļu un pierakstieties ar globālā administratora vai drošības administratora kontu.</span><span class="sxs-lookup"><span data-stu-id="22335-109">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="22335-110">Kreisajā navigācijas rūtī sadaļā Apdraudējumu **pārvaldība izvēlieties** Politikas **un** \> **Seifs saites**.</span><span class="sxs-lookup"><span data-stu-id="22335-110">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="22335-111">Sadaļā **Politikas, kas attiecas uz visu organizāciju** atlasiet šo politiku un noklikšķiniet uz **Rediģēt.**</span><span class="sxs-lookup"><span data-stu-id="22335-111">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="22335-112">Sadaļā **Iestatījumi** **iespējojiet Opciju Lietot drošās saites ziņojumiem, kas nosūtīti organizācijā.**</span><span class="sxs-lookup"><span data-stu-id="22335-112">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
