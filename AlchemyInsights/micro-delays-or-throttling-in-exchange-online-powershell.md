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
ms.openlocfilehash: 6753dcb375ea5e19b01c4350b61aa8904aa102112df175a3f70281d18a634dbf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098573"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Exchange Online PowerShell mikro aiztures vai ierobežošana

Palaižot skriptus vai komandlietotnes Exchange Online, jums var tikt parādīts paziņojums “Piemērotas mikro aiztures” vai piemērota ierobežošana. Lūk, daži ieteikumi, kā to novērst:

- Lūdzu, palaidiet mūsu diagnostiku, lai atslābtu nomnieka PowerShell ierobežošanas politikas. Šis risinājums atrisinās problēmu lielākajai daļai.
- Ja problēmu joprojām nevar atrisināt, izmantojiet [Exchange Online v2 PowerShell](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)moduli, kurā iekļauti CMDlets, kuru pamatā ir REST API un kuri ir ievērojami efektīvāki. Šis varētu būt lielisks risinājums daudzām bieži izmantotām Get- komandlietotnēm.
- Ja vēlaties izmantot CMDlets, kas nav apskatītas v2 modulī, lūdzu, skatiet rakstu [PowerShell cmdlet](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)izpildīšana lielam lietotāju skaitam programmā Office 365, kurā ir ietvertas sarunas par PowerShell ierobežošanas ierobežojumu apiet Exchange Online.
