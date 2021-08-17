---
title: Exchange Online PowerShell mikro aiztures vai ierobežošana
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
- "3500011"
- "5106"
ms.openlocfilehash: 2fab21f76f455815979ae162c1ce8246ad5c297e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314707"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Exchange Online PowerShell mikro aiztures vai ierobežošana

Palaižot skriptus vai komandlietotnes Exchange Online, jums var tikt parādīts paziņojums “Piemērotas mikro aiztures” vai piemērota ierobežošana. Lūk, daži ieteikumi, kā to novērst:

- Lūdzu, palaidiet mūsu diagnostiku, lai atslābtu nomnieka PowerShell ierobežošanas politikas. Šis risinājums atrisinās lielāko daļu problēmu.
- Ja problēmu joprojām nevar atrisināt, izmantojiet [Exchange Online v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)moduli, kurā iekļauti CMDlets, kuru pamatā ir REST API un kuri ir ievērojami efektīvāki. Šis varētu būt lielisks risinājums daudzām bieži izmantotām Get- komandlietotnēm.
- Ja vēlaties izmantot CMDlets, kas nav apskatītas v2 modulī, lūdzu, skatiet rakstu [PowerShell cmdlet](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)izpildīšana lielam lietotāju skaitam programmā Office 365, kurā ir ietvertas sarunas par PowerShell ierobežošanas ierobežojumu apiešanas Exchange Online.
