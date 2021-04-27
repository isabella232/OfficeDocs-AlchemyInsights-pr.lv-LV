---
title: PST importēšanas problēmu novēršana
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
- "1800027"
- "1225"
ms.openlocfilehash: 5065b9895954371e4298c98e8aadb67ba8f140fd
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/27/2021
ms.locfileid: "52059822"
---
# <a name="troubleshooting-pst-import-issues"></a>PST importēšanas problēmu novēršana

- Ja importējat Pašā Outlook klientā, skatiet rakstu [Outlook .pst faila importēšanas problēmu novēršana.](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)

- Ja izmantojat importēšanas pakalpojumu un tas iestrēgst, ņemiet vērā, ka katrs PST fails, ko augšupielādējat Azure krātuves atrašanās vietā, nedrīkst būt lielāks par 20 GB. PST faili, kas ir lielāki par 20 GB, var ietekmēt PST importēšanas procesa veiktspēju. Lai iegūtu papildinformāciju par problēmu novēršanu saistībā ar [iestrēgušiem darbiem, skatiet rakstu Problēmas, kas ietekmē PST importēšanas darbus.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)

- Ja vēlaties pārbaudīt konkrēta importēšanas darba statusu, izmantojiet [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Pilnu informāciju par importēšanas pakalpojumu skatiet [rakstā Pārskats par organizācijas PST failu importēšanu.](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)
