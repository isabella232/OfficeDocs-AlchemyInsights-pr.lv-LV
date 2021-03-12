---
title: Problēmas ar Microsoft Defender instalēšanu Mac vai Linux ierīcē
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
ms.openlocfilehash: a8d5ad2246b9b83e1e0a4d5be4dd8bb41c16e734
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713838"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a><span data-ttu-id="9eaf0-102">Problēmas ar Microsoft Defender instalēšanu Mac vai Linux ierīcē</span><span class="sxs-lookup"><span data-stu-id="9eaf0-102">Issues installing Microsoft Defender on Mac or Linux</span></span>

<span data-ttu-id="9eaf0-103">**Mac**</span><span class="sxs-lookup"><span data-stu-id="9eaf0-103">**Mac**</span></span>

- <span data-ttu-id="9eaf0-104">Nodrošiniet, lai tiktu ievērotas sistēmas prasības pirms Microsoft Defender ATP for Mac instalēšanas.</span><span class="sxs-lookup"><span data-stu-id="9eaf0-104">Ensure that system requirements are met before installing Microsoft Defender ATP for Mac.</span></span> <span data-ttu-id="9eaf0-105">Papildinformāciju skatiet rakstā [Microsoft Defender ATP darbam ar Mac instalēšana](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span><span class="sxs-lookup"><span data-stu-id="9eaf0-105">For more info, see [How to install Microsoft Defender ATP for Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span></span>  
- <span data-ttu-id="9eaf0-106">Pārskatiet informāciju failā: "/Library/Logs/Microsoft/mdatp/install.log".</span><span class="sxs-lookup"><span data-stu-id="9eaf0-106">Review the information in the file: "/Library/Logs/Microsoft/mdatp/install.log".</span></span>

<span data-ttu-id="9eaf0-107">**Linux**</span><span class="sxs-lookup"><span data-stu-id="9eaf0-107">**Linux**</span></span>

- <span data-ttu-id="9eaf0-108">Nodrošiniet, lai tiktu ievērotas sistēmas prasības pirms Microsoft Defender ATP darbam ar Linux instalēšanas.</span><span class="sxs-lookup"><span data-stu-id="9eaf0-108">Ensure that system requirements are met before installing Microsoft Defender ATP for Linux.</span></span> <span data-ttu-id="9eaf0-109">Papildinformāciju skatiet rakstā [Microsoft Defender ATP For Linux instalēšana](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span><span class="sxs-lookup"><span data-stu-id="9eaf0-109">For more info, see [How to install Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span> 
- <span data-ttu-id="9eaf0-110">Lai pārliecinātos, vai MDATP pakalpojums darbojas, skatiet rakstu [instalēšana neizdevās](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).</span><span class="sxs-lookup"><span data-stu-id="9eaf0-110">To verify that MDATP service is running, see [Installation failed](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).</span></span>  
    <span data-ttu-id="9eaf0-111">Lai novērstu un atrisinātu problēmas, ja pakalpojums nedarbojas, skatiet darbības, [kas jāveic, lai novērstu problēmas, ja mdatp pakalpojums nedarbojas](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span><span class="sxs-lookup"><span data-stu-id="9eaf0-111">To troubleshoot and resolve issues if the service is not running, see [Steps to troubleshoot if mdatp service isn't running](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span></span>
- <span data-ttu-id="9eaf0-112">Lai uzzinātu, kādas darbības ir jāveic, lai pārbaudītu klienta konfigurāciju, kas pārbauda produkta darbspēju un EICAR teksta failu, skatiet rakstu [klienta konfigurācija](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span><span class="sxs-lookup"><span data-stu-id="9eaf0-112">For steps to check the client configuration, which verifies the health of the product, and to run a detection test on the EICAR text file, see [Client configuration](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span></span>  

    <span data-ttu-id="9eaf0-113">**Piezīmes** Atbalstīto failu sistēmu sarakstu par darbībām, kas attiecas uz piekļuvi, skatiet rakstā [Microsoft Defender ATP darbam ar Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span><span class="sxs-lookup"><span data-stu-id="9eaf0-113">**Note** For a list of supported file systems for on-access activity, see [Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span>