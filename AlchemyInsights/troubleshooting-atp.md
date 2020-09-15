---
title: Problēmu novēršana saistībā ar Office 365 Advanced Threat Protection
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
ms.openlocfilehash: 5a13653ba08d8c6b822354ff70f6d276d31cd816
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658921"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a><span data-ttu-id="a30b5-102">Problēmu novēršana saistībā ar Office 365 Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="a30b5-102">Troubleshooting Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="a30b5-103">Vai pamanīsit ziņojumu piegādes kavējumus?</span><span class="sxs-lookup"><span data-stu-id="a30b5-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="a30b5-104">Izmantojiet [dinamiskās piegādes](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) opciju savā ATP drošas pielikumu politikā.</span><span class="sxs-lookup"><span data-stu-id="a30b5-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="a30b5-105">Tas palīdzēs izvairīties no ziņojumu kavējumiem, aizsargājot adresātus no ļaunprātīgiem failiem.</span><span class="sxs-lookup"><span data-stu-id="a30b5-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="a30b5-106">Vai vēlaties, lai Microsoft ziņotu par aplamiem pozitīviem vai viltus negatīviem?</span><span class="sxs-lookup"><span data-stu-id="a30b5-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="a30b5-107">Izmantojiet šo [saiti](https://www.microsoft.com/wdsi/filesubmission/) , lai iesniegtu analīzes failus.</span><span class="sxs-lookup"><span data-stu-id="a30b5-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="a30b5-108">Vai zinājāt, ka varat iespējot drošu saišu aizsardzību iekšējiem e-pasta ziņojumiem, kas tiek sūtīti starp adresātiem jūsu organizācijā?</span><span class="sxs-lookup"><span data-stu-id="a30b5-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="a30b5-109">Izpildiet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="a30b5-109">Follow these steps:</span></span>

  1. <span data-ttu-id="a30b5-110">Dodieties uz [https://protection.office.com](https://protection.office.com) un pierakstieties, izmantojot globālo administratora vai drošības administratora kontu.</span><span class="sxs-lookup"><span data-stu-id="a30b5-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="a30b5-111">Kreisajā navigācijas rūtī sadaļā **draudu pārvaldība**izvēlieties **politikas** \> **drošās saites**.</span><span class="sxs-lookup"><span data-stu-id="a30b5-111">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="a30b5-112">Politikas, **kas attiecas uz visu organizāciju** sadaļu, atlasiet politiku un noklikšķiniet uz **Rediģēt**.</span><span class="sxs-lookup"><span data-stu-id="a30b5-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="a30b5-113">Sadaļā **Iestatījumi**iespējojiet **lietot drošas saites ziņojumiem, kas tiek sūtīti organizācijā**.</span><span class="sxs-lookup"><span data-stu-id="a30b5-113">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
