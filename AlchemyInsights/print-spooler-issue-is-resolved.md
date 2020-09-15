---
title: Ir novērsta drukas spolēšanas problēma
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 66b39434ef6f9ad2b8392f811704e67c1bcffd2b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801848"
---
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="ee15a-102">Ir novērsta drukas spolēšanas problēma</span><span class="sxs-lookup"><span data-stu-id="ee15a-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="ee15a-103">Ja jūsu ierīce ir atjaunināta ar Windows 10  **OS būvējumu 19041,329**, iespējams, esat pamanījis problēmu, kad noteikti printeri netiek drukāti.</span><span class="sxs-lookup"><span data-stu-id="ee15a-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="ee15a-104">Drukas spolētājs var atklāt kļūdu vai negaidīti aizvērt, kad mēģināt drukāt, un neviens rezultāts nav no skartā printera.</span><span class="sxs-lookup"><span data-stu-id="ee15a-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="ee15a-105">Šī problēma ir novērsta OS būvējumā  **19041,331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span><span class="sxs-lookup"><span data-stu-id="ee15a-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="ee15a-106">**Notiekošā izmeklēšana**</span><span class="sxs-lookup"><span data-stu-id="ee15a-106">**Ongoing investigation**</span></span>

<span data-ttu-id="ee15a-107">Lokālā drošības iestādes apakšsistēmas pakalpojuma (LSASS) fails (**Isass.exe**), iespējams, neizdosies dažās ierīcēs ar kļūdas ziņojumu "kritiska sistēmas darbība, C:\WINDOWS\system32\Isass.exe, neizdevās ar statusa koda c0000008.</span><span class="sxs-lookup"><span data-stu-id="ee15a-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="ee15a-108">Tagad ir jārestartē dators.</span><span class="sxs-lookup"><span data-stu-id="ee15a-108">The machine must now be restarted".</span></span>  <span data-ttu-id="ee15a-109">**Microsoft strādā pie izšķirtspējas un piedāvās atjauninājumu gaidāmajā laidienā.**</span><span class="sxs-lookup"><span data-stu-id="ee15a-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="ee15a-110">Lai iegūtu papildinformāciju, lūdzu, skatiet rakstu  [Windows 10 versija 2004 zināmās problēmas](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span><span class="sxs-lookup"><span data-stu-id="ee15a-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>