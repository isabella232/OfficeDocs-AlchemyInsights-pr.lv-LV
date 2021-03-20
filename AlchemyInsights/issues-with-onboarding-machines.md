---
title: Problēmas ar pievienošanas mašīnām Microsoft Defender galapunktiem
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901574"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a><span data-ttu-id="c78d1-102">Problēmas ar pievienošanas mašīnām Microsoft Defender galapunktiem</span><span class="sxs-lookup"><span data-stu-id="c78d1-102">Issues with onboarding machines to Microsoft Defender for Endpoints</span></span>

<span data-ttu-id="c78d1-103">Jums var rasties problēmas pievienošanas mašīnām ar MDE pakalpojumam.</span><span class="sxs-lookup"><span data-stu-id="c78d1-103">You might have issues with onboarding machines to MDE service.</span></span> <span data-ttu-id="c78d1-104">Ja varat piekļūt lietotāja mašīnai, veiciet tālāk norādītās darbības:</span><span class="sxs-lookup"><span data-stu-id="c78d1-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="c78d1-105">Lejupielādējiet jaunāko [MDE klienta analīzes priekšskatījuma versijas](https://aka.ms/betamdeanalyzer) diagnostikas rīku.</span><span class="sxs-lookup"><span data-stu-id="c78d1-105">Download the latest preview version of the [MDE Client Analyzer](https://aka.ms/betamdeanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="c78d1-106">Ar peles labo pogu noklikšķiniet uz **MDEClientAnalyzer.cmd** un atlasiet ‘Run as administrator’ (‘Palaist kā administratoram’).</span><span class="sxs-lookup"><span data-stu-id="c78d1-106">Right click **MDEClientAnalyzer.cmd** and select ‘Run as administrator’.</span></span>
3. <span data-ttu-id="c78d1-107">Sekojiet norādījumiem, kas ieteikti **MDEClientAnalyzer.htm**.</span><span class="sxs-lookup"><span data-stu-id="c78d1-107">Follow any guidance suggested in **MDEClientAnalyzer.htm**.</span></span>
4. <span data-ttu-id="c78d1-108">Lai iegūtu papildu izvērstākus žurnālus, pārskatiet izveidoto apakšmapi ar nosaukumu **MDEClientAnalyzerResult**.</span><span class="sxs-lookup"><span data-stu-id="c78d1-108">For more verbose logs, review the created sub-folder named **MDEClientAnalyzerResult**.</span></span>
5. <span data-ttu-id="c78d1-109">Ja nepieciešami papildu norādījumi, sazinieties ar [Microsoft Defender uzlaboto pretdraudu aizsardzību](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support), un nodrošiniet iegūto MDEClientAnalyzerResult.zip failu analīzei.</span><span class="sxs-lookup"><span data-stu-id="c78d1-109">If additional guidance is needed, contact [Microsoft Defender for Endpoint support](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) and provide the resulting MDEClientAnalyzerResult.zip file for analysis.</span></span>
