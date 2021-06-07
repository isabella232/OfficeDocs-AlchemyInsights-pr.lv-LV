---
title: Microsoft Defender galapunkta veiktspējas problēmas operētājsistēmā Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794005"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="ff73b-102">Microsoft Defender galapunkta veiktspējas problēmas operētājsistēmā Linux</span><span class="sxs-lookup"><span data-stu-id="ff73b-102">Performance issues for Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="ff73b-103">Šajā rakstā ir norādījumi, kā noteikt veiktspējas problēmas programmatūrai Microsoft Defender galapunktam operētājsistēmā Linux.</span><span class="sxs-lookup"><span data-stu-id="ff73b-103">This article guides you through the steps of identifying performance issues for Microsoft Defender for Endpoint on Linux.</span></span>

<span data-ttu-id="ff73b-104">Vispirms pārbaudiet, vai problēma ir novērsta, izmantojot [jaunāko versiju.](/microsoft-365/security/defender-endpoint/linux-whatsnew)</span><span class="sxs-lookup"><span data-stu-id="ff73b-104">It's important to first verify that the problem you're experiencing is resolved with the [latest version](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span></span> 

<span data-ttu-id="ff73b-105">Lai sāktu izpēti, skatiet rakstu [Microsoft Defender galapunkta veiktspējas problēmu novēršana operētājsistēmā Linux.](/microsoft-365/security/defender-endpoint/linux-support-perf)</span><span class="sxs-lookup"><span data-stu-id="ff73b-105">To start your investigation, see [Troubleshoot performance issues for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span></span>

## <a name="exclusions"></a><span data-ttu-id="ff73b-106">Izņēmumi</span><span class="sxs-lookup"><span data-stu-id="ff73b-106">Exclusions</span></span>

<span data-ttu-id="ff73b-107">Izņēmumi var palīdzēt mazināt veiktspējas problēmas.</span><span class="sxs-lookup"><span data-stu-id="ff73b-107">Exclusions can help to mitigate performance issues.</span></span> <span data-ttu-id="ff73b-108">Pirms sākat darbu, pārskatiet izņēmumus, lai visi papildu riski būtu zināmi un dokumentēti.</span><span class="sxs-lookup"><span data-stu-id="ff73b-108">Review your exclusions before you begin so any additional risk is known and documented.</span></span>

<span data-ttu-id="ff73b-109">Papildinformāciju skatiet rakstā [Microsoft Defender galapunkta izņēmumu konfigurēšana](/microsoft-365/security/defender-endpoint/linux-exclusions)un pārbaude operētājsistēmā Linux.</span><span class="sxs-lookup"><span data-stu-id="ff73b-109">For more information, see [Configure and validate exclusions for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span></span>

<span data-ttu-id="ff73b-110">Ja ir vairāki faili& vai mapes izslēgt, un tie visi atrodas vienā vietā, iespējams, vieglāk ir izslēgt no kalnpunkta.</span><span class="sxs-lookup"><span data-stu-id="ff73b-110">When you have multiple files & folders to exclude and they're all on the same mountpoint, it might be easier to exclude the mountpoint.</span></span> <span data-ttu-id="ff73b-111">Sākot ar februāra laidienu 101.22.80, varat izslēgt visu mountpoint.</span><span class="sxs-lookup"><span data-stu-id="ff73b-111">Starting with February release 101.22.80, you can exclude an entire mountpoint.</span></span>

<span data-ttu-id="ff73b-112">Piemēram, ja /mnt/backup ir mountpoint, varat pievienot /mnt/backup izslēgšanas sarakstam, izpildot šo komandu:</span><span class="sxs-lookup"><span data-stu-id="ff73b-112">For example, if /mnt/backup is a mountpoint, you can add /mnt/backup to the exclude list by running this command:</span></span>

`$ mdatp exclusion folder add –path /mnt/backup`

<span data-ttu-id="ff73b-113">**Piezīme.** Pievienojot izņēmumus, tiek palielināts risks, ka ļaunprogrammatūra netiek noteikta, un tā ir jāapstrādā un ieviesīs rūpīgi.</span><span class="sxs-lookup"><span data-stu-id="ff73b-113">**Note**: Adding exclusions increases the risk of malware not being detected and should be handled and implemented with care.</span></span>

## <a name="need-help"></a><span data-ttu-id="ff73b-114">Vai nepieciešama palīdzība?</span><span class="sxs-lookup"><span data-stu-id="ff73b-114">Need Help?</span></span>

<span data-ttu-id="ff73b-115">Lai jums palīdzētu efektīvāk, apkopojiet diagnostikas datus pirms atbalsta pieteikuma atvēršanas.</span><span class="sxs-lookup"><span data-stu-id="ff73b-115">To assist you in the most efficient way, collect the diagnostic data before opening a support case.</span></span>
