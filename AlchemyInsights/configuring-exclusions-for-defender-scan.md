---
title: Microsoft Defender ATP atstumtības konfigurēšana
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
- "6027"
- "9001464"
ms.openlocfilehash: 912e77b9b1a149fef373f2d0814fb2f0671a48c6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713898"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="ac4ca-102">Microsoft Defender ATP atstumtības konfigurēšana</span><span class="sxs-lookup"><span data-stu-id="ac4ca-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="ac4ca-103">Vispārīgi varat izslēgt noteiktus failu paplašinājumus un mapju atrašanās vietas, izmantojot Microsoft Defender ATP skenēšanu.</span><span class="sxs-lookup"><span data-stu-id="ac4ca-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="ac4ca-104">Varat arī konfigurēt izņēmumus failiem, kas atvērti noteiktos procesos.</span><span class="sxs-lookup"><span data-stu-id="ac4ca-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="ac4ca-105">Papildinformāciju skatiet rakstā [izslēgšanas konfigurēšana un pārbaude, ņemot vērā faila paplašinājumu un mapes atrašanās vietu](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) , kā arī [tādu failu izslēgšanas konfigurēšana, kas atvērti, izmantojot procesus](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span><span class="sxs-lookup"><span data-stu-id="ac4ca-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="ac4ca-106">Lai konfigurētu izņēmumus sistēmai  **Windows server 2016 un 2019**, skatiet rakstu [Microsoft Defender Antivirus izslēgšanu konfigurēšana operētājsistēmā Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="ac4ca-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="ac4ca-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="ac4ca-107">**Mac**</span></span>

<span data-ttu-id="ac4ca-108">Detalizētu informāciju par atbalstītajiem izslēgšanas tipiem un saraksta konfigurēšanu operētājsistēmā Mac skatiet rakstā [atbalstītie izņēmumu tipi](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) un to, [kā konfigurēt izņēmumu sarakstu](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span><span class="sxs-lookup"><span data-stu-id="ac4ca-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="ac4ca-109">**Piezīmes** Varat arī validēt izņēmumu sarakstus, izmantojot EICAR testa failu.</span><span class="sxs-lookup"><span data-stu-id="ac4ca-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="ac4ca-110">Papildinformāciju skatiet rakstā [izņēmumu sarakstu pārbaude, izmantojot EICAR testa failu](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="ac4ca-110">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="ac4ca-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="ac4ca-111">**Linux**</span></span>

<span data-ttu-id="ac4ca-112">Detalizētu informāciju par atbalstītajiem izslēgšanas tipiem un to, kā konfigurēt sarakstu ar Linux izslēgšanu, skatiet sadaļā [atbalstītie izslēgšanas tipi](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) un [konfigurējiet un validējiet Microsoft Defender ATP For Linux izņēmumus](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span><span class="sxs-lookup"><span data-stu-id="ac4ca-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="ac4ca-113">**Piezīmes** Varat arī validēt izņēmumu sarakstus, izmantojot EICAR testa failu.</span><span class="sxs-lookup"><span data-stu-id="ac4ca-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="ac4ca-114">Papildinformāciju skatiet rakstā [izņēmumu sarakstu pārbaude, izmantojot EICAR testa failu](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="ac4ca-114">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 