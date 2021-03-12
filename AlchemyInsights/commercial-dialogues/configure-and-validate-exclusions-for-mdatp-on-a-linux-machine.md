---
title: Izslēgšanas MDATP konfigurēšana un pārbaude Linux datorā
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4fad0a513f7c6d2f0337019488a4055c25e1650d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746020"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a><span data-ttu-id="c9788-102">Izslēgšanas MDATP konfigurēšana un pārbaude Linux datorā</span><span class="sxs-lookup"><span data-stu-id="c9788-102">Configure and validate exclusions for MDATP on a Linux machine</span></span>

<span data-ttu-id="c9788-103">Varat izslēgt noteiktus failus, mapes, procesus un procesa atvērtos failus no MDATP skenē.</span><span class="sxs-lookup"><span data-stu-id="c9788-103">You can exclude certain files, folders, processes, and process-opened files from MDATP scans.</span></span> <span data-ttu-id="c9788-104">Izņēmumi palīdz nepareizi noteikt, vai jūsu organizācijai ir unikāli vai pielāgoti programmatūras un faili.</span><span class="sxs-lookup"><span data-stu-id="c9788-104">Exclusions help prevent incorrect detection of software and files unique or customized to your organization.</span></span> <span data-ttu-id="c9788-105">Izņēmumi palīdz arī samazināt MDATP izraisītās veiktspējas problēmas.</span><span class="sxs-lookup"><span data-stu-id="c9788-105">Exclusions also help mitigate performance problems caused by MDATP.</span></span>

<span data-ttu-id="c9788-106">Lai uzzinātu vairāk, skatiet rakstu [MDATP For Linux konfigurēšana un validācija](https://go.microsoft.com/fwlink/?linkid=2144517).</span><span class="sxs-lookup"><span data-stu-id="c9788-106">To learn more, see [Configure and validate exclusions for MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="c9788-107">Šajā rakstā aprakstītie izņēmumi neattiecas uz citām MDATP iespējām darbam ar Linux, tostarp galapunkta noteikšanu un reaģēšanu (EDR).</span><span class="sxs-lookup"><span data-stu-id="c9788-107">The exclusions described in this article don't apply to other capabilities of MDATP for Linux, including endpoint detection and response (EDR).</span></span> <span data-ttu-id="c9788-108">Faili, kurus izslēdzat, izmantojot šajā rakstā aprakstītās metodes, joprojām var aktivizēt EDR brīdinājumus un citas atklāšanas iespējas.</span><span class="sxs-lookup"><span data-stu-id="c9788-108">Files that you exclude by using the methods described in this article can still trigger EDR alerts and other detection capabilities.</span></span>
