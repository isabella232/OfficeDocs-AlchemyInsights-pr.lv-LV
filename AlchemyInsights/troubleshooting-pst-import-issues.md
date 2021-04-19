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
ms.openlocfilehash: 07609b39149c003b029f3ea5669f4044af43c25d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826170"
---
# <a name="troubleshooting-pst-import-issues"></a>PST importēšanas problēmu novēršana

- Ja importējat pats Outlook klientā, skatiet rakstu [Problēmu novēršana saistībā ar Outlook.pst faila](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Ja izmantojat importēšanas pakalpojumu un tas ir iestrēdzis, ņemiet vērā, ka katrs PST fails, kas tiek augšupielādēts Azure krātuves atrašanās vietā, nedrīkst būt lielāks par 20 GB. PST faili, kas lielāki par 20 GB, var ietekmēt PST importēšanas procesa veiktspēju.

- Ja vēlaties pārbaudīt konkrētu importēšanas darba statusu, varat izmantot [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Lai iegūtu pilnu informāciju par importēšanas pakalpojumu, lūdzu, skatiet [Pārskats par savas organizācijas PST failu importēšanu](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).
