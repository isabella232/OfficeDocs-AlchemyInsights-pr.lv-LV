---
title: Pakalpojuma importēšanas darba iestrēgināšanas problēmu novēršana
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: 987383037f843d347477c0becc859c663736a676
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/27/2021
ms.locfileid: "52125487"
---
# <a name="troubleshooting-import-service-job-stuck"></a><span data-ttu-id="429ac-102">Pakalpojuma importēšanas darba iestrēgināšanas problēmu novēršana</span><span class="sxs-lookup"><span data-stu-id="429ac-102">Troubleshooting Import Service job stuck</span></span>

<span data-ttu-id="429ac-103">Ja rodas problēmas, kuru dēļ importēšanas pakalpojumu darbi ir iestrēguši vai rodas kļūmes, pārbaudiet un mēģiniet veikt šādas darbības:</span><span class="sxs-lookup"><span data-stu-id="429ac-103">If you are experiencing issues with Import service jobs stuck or failing, examine and try the following:</span></span>

- <span data-ttu-id="429ac-104">Pārskatiet PST faila lielumu.</span><span class="sxs-lookup"><span data-stu-id="429ac-104">Review the size of of the PST file.</span></span> <span data-ttu-id="429ac-105">Maksimālais importējot ieteicamais PST faila lielums ir 20 GB.</span><span class="sxs-lookup"><span data-stu-id="429ac-105">The maximum recommended size of a PST file for import is 20GB.</span></span>

- <span data-ttu-id="429ac-106">Ja pastāv aizdomas, ka izlaistie vienumi ir bojāti, Scanpst.exe un labojiet kļūdas PST failos.</span><span class="sxs-lookup"><span data-stu-id="429ac-106">If you suspect skipped items due to corruption, run Scanpst.exe to diagnose and fix errors in PST files.</span></span>

- <span data-ttu-id="429ac-107">Ja importēšanas laikā tiek parādīts kļūdas ziņojums "MapiExceptionShutoffQuotaExceeded", pārliecinieties, vai mērķa pastkastei ir pietiekama noslodze, lai importētu vajadzīgos PST failus.</span><span class="sxs-lookup"><span data-stu-id="429ac-107">If you see a "MapiExceptionShutoffQuotaExceeded" error during import, make sure the target mailbox has sufficient capacity to import the desired PST files.</span></span>

<span data-ttu-id="429ac-108">Papildinformāciju par PST importēšanas darba problēmu novēršanu skatiet rakstā [PST importēšanas darbu problēmu novēršana.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)</span><span class="sxs-lookup"><span data-stu-id="429ac-108">For more information on troubleshooting PST import job issues, see [Troubleshoot issues with PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

<span data-ttu-id="429ac-109">Informāciju par to, kā novērst problēmas, importējot PST failus programmā Outlook, skatiet rakstā Ar [.pst Outlook faila (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us)importēšanu saistītas problēmas.</span><span class="sxs-lookup"><span data-stu-id="429ac-109">For information about how to fix issues when importing PSTs into Outlook, see [Fix problems importing an Outlook .pst file (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span></span>