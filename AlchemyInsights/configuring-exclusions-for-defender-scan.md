---
title: Izņēmumu konfigurēšana skenēšanai Microsoft Defender ATP konfigurēšana
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
ms.openlocfilehash: 5eb18f4133aca93c1506f4975c8d0567bede8d57
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543692"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="b058f-102">Izņēmumu konfigurēšana skenēšanai Microsoft Defender ATP konfigurēšana</span><span class="sxs-lookup"><span data-stu-id="b058f-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="b058f-103">Lai skenētu, kopumā varat izslēgt noteiktus failu paplašinājumus un Microsoft Defender ATP atrašanās vietas.</span><span class="sxs-lookup"><span data-stu-id="b058f-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="b058f-104">Varat arī konfigurēt izņēmumus failiem, kas atvērti noteiktos procesos.</span><span class="sxs-lookup"><span data-stu-id="b058f-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="b058f-105">Papildinformāciju skatiet rakstā Izņēmumu konfigurēšana un pārbaude, pamatojoties uz faila paplašinājumu un mapes [atrašanās](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) vietu un Izņēmumu konfigurēšana [failiem, kurus atver procesi.](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="b058f-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="b058f-106">Lai konfigurētu izņēmumus **Windows Server 2016 un 2019**, skatiet [rakstu pretvīrusu programmatūra Microsoft Defender izņēmumu konfigurēšana Windows serverī.](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="b058f-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="b058f-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="b058f-107">**Mac**</span></span>

<span data-ttu-id="b058f-108">Detalizētu informāciju par atbalstītajiem izņēmumu tipiem un izņēmumu [](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) sarakstu konfigurēšanu Mac datoriem skatiet sadaļā Atbalstītie izņēmumu tipi un Kā [konfigurēt izņēmumu sarakstu.](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions)</span><span class="sxs-lookup"><span data-stu-id="b058f-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="b058f-109">**Piezīme** Varat arī validēt izņēmumu sarakstus, izmantojot EICAR testa failu.</span><span class="sxs-lookup"><span data-stu-id="b058f-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="b058f-110">Papildinformāciju skatiet [rakstā Izņēmumu sarakstu pārbaude, izmantojot EICAR testa failu.](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="b058f-110">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="b058f-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="b058f-111">**Linux**</span></span>

<span data-ttu-id="b058f-112">Detalizētu informāciju par atbalstītajiem izslēgšanas tipiem un linux [](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) izņēmumu saraksta konfigurēšanu skatiet rakstā Atbalstītie izņēmumu tipi un Programmas Microsoft Defender ATP operētājsistēmai Linux izņēmumu [konfigurēšana un pārbaude.](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions)</span><span class="sxs-lookup"><span data-stu-id="b058f-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="b058f-113">**Piezīme** Varat arī validēt izņēmumu sarakstus, izmantojot EICAR testa failu.</span><span class="sxs-lookup"><span data-stu-id="b058f-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="b058f-114">Papildinformāciju skatiet [rakstā Izņēmumu sarakstu pārbaude, izmantojot EICAR testa failu.](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="b058f-114">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 