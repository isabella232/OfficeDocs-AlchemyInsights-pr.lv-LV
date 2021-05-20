---
title: Problēmas ar Microsoft Defender instalēšanu Mac vai Linux operētājsistēmā
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 39f180852fd0438597fa1ce665b2703fbc7b1aa4
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539687"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a><span data-ttu-id="3d7a6-102">Problēmas ar Microsoft Defender instalēšanu Mac vai Linux operētājsistēmā</span><span class="sxs-lookup"><span data-stu-id="3d7a6-102">Issues installing Microsoft Defender on Mac or Linux</span></span>

<span data-ttu-id="3d7a6-103">**Mac**</span><span class="sxs-lookup"><span data-stu-id="3d7a6-103">**Mac**</span></span>

- <span data-ttu-id="3d7a6-104">Pārliecinieties, vai sistēmas prasības ir izpildītas, pirms instalējat Microsoft Defender ATP for Mac.</span><span class="sxs-lookup"><span data-stu-id="3d7a6-104">Ensure that system requirements are met before installing Microsoft Defender ATP for Mac.</span></span> <span data-ttu-id="3d7a6-105">Papildinformāciju skatiet rakstā [Kā instalēt Microsoft Defender ATP for Mac](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span><span class="sxs-lookup"><span data-stu-id="3d7a6-105">For more info, see [How to install Microsoft Defender ATP for Mac](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span></span>  
- <span data-ttu-id="3d7a6-106">Pārskatiet informāciju failā: "/Library/Logs/Microsoft/mdatp/install.log".</span><span class="sxs-lookup"><span data-stu-id="3d7a6-106">Review the information in the file: "/Library/Logs/Microsoft/mdatp/install.log".</span></span>

<span data-ttu-id="3d7a6-107">**Linux**</span><span class="sxs-lookup"><span data-stu-id="3d7a6-107">**Linux**</span></span>

- <span data-ttu-id="3d7a6-108">Pārliecinieties, vai sistēmas prasības ir izpildītas, Microsoft Defender ATP operētājsistēmai Linux.</span><span class="sxs-lookup"><span data-stu-id="3d7a6-108">Ensure that system requirements are met before installing Microsoft Defender ATP for Linux.</span></span> <span data-ttu-id="3d7a6-109">Papildinformāciju skatiet [rakstā MDATP instalēšana linux lietojumprogrammai.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)</span><span class="sxs-lookup"><span data-stu-id="3d7a6-109">For more info, see [How to install MDATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span> 
- <span data-ttu-id="3d7a6-110">Lai pārbaudītu, vai darbojas MDATP pakalpojums, skatiet rakstu [Instalēšana neizdevās.](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)</span><span class="sxs-lookup"><span data-stu-id="3d7a6-110">To verify that MDATP service is running, see [Installation failed](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).</span></span>  
    <span data-ttu-id="3d7a6-111">Lai novērstu un novērstu problēmas, ja pakalpojums nedarbojas, skatiet rakstu Darbības, lai novērstu problēmas, ja [nedarbojas mdatp pakalpojums.](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)</span><span class="sxs-lookup"><span data-stu-id="3d7a6-111">To troubleshoot and resolve issues if the service is not running, see [Steps to troubleshoot if mdatp service isn't running](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span></span>
- <span data-ttu-id="3d7a6-112">Lai uzzinātu, kādas darbības ir jāveic, lai pārbaudītu klienta konfigurāciju, kas pārbauda produkta darbspēju un izpildītu noteikšanas testu EICAR teksta failā, skatiet rakstu [Klienta konfigurācija.](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration)</span><span class="sxs-lookup"><span data-stu-id="3d7a6-112">For steps to check the client configuration, which verifies the health of the product, and to run a detection test on the EICAR text file, see [Client configuration](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span></span>  

    <span data-ttu-id="3d7a6-113">**Piezīme** Atbalstīto failu sistēmu sarakstu par piekļuves darbībām skatiet sadaļā [Microsoft Defender ATP operētājsistēmai Linux.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)</span><span class="sxs-lookup"><span data-stu-id="3d7a6-113">**Note** For a list of supported file systems for on-access activity, see [Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span>