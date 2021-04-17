---
title: EWS ierobežošanas iestatījumu maiņa
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 16916d5f16f763d87ce0d5ef830e741279c9f4df
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818043"
---
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="873a2-102">EWS ierobežošanas iestatījumu maiņa</span><span class="sxs-lookup"><span data-stu-id="873a2-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="873a2-103">Lūdzu, veiciet mūsu automatizēto testu, kas atļauj mainīt EWS ierobežošanas politiku, kamēr notiek jūsu migrācija.</span><span class="sxs-lookup"><span data-stu-id="873a2-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="873a2-104">Ņemiet vērā, ka pat pēc šīs palaišanas EWS importēšana joprojām būs ierobežota līdz 150 mb 5 minūtēs vienai pastkastei. Lai panāktu lielāku migrācijas caurlaidspējas ātrumu, lūdzu, migrējiet vairāk lietotāju vienlaikus.</span><span class="sxs-lookup"><span data-stu-id="873a2-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="873a2-105">Lūdzu, ņemiet vērā, ka EWS ierobežošanas politikas izmaiņas neietekmē šādus migrācijas tipus (lietojot Microsoft rīkus): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G komplekts, publiskā mape vai PST importēšanas pakalpojums.</span><span class="sxs-lookup"><span data-stu-id="873a2-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>