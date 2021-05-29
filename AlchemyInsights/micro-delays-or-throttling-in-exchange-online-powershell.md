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
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702133"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Exchange Online PowerShell mikro aiztures vai ierobežošana

Palaižot skriptus vai komandlietotnes Exchange Online, jums var tikt parādīts paziņojums “Piemērotas mikro aiztures” vai piemērota ierobežošana. Lūk, daži ieteikumi, kā to novērst:

- Lūdzu, palaidiet mūsu diagnostiku, lai atslābtu nomnieka PowerShell ierobežošanas politikas. Šis risinājums atrisinās problēmu lielākajai daļai.
- Ja problēmu joprojām nevar atrisināt, izmantojiet [Exchange Online v2 PowerShell](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)moduli, kurā iekļauti CMDlets, kuru pamatā ir REST API un kuri ir ievērojami efektīvāki. Šis varētu būt lielisks risinājums daudzām bieži izmantotām Get- komandlietotnēm.
- Ja vēlaties izmantot CMDlets, kas nav apskatītas v2 modulī, lūdzu, skatiet rakstu [PowerShell cmdlet](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)izpildīšana lielam lietotāju skaitam programmā Office 365, kurā ir ietvertas sarunas par PowerShell ierobežošanas ierobežojumu apiet Exchange Online.
