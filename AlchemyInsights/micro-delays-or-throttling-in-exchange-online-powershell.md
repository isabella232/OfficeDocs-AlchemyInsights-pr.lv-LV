---
title: Exchange Online PowerShell mikro aiztures vai ierobežošana
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 7ab4e7f18b7b8edf08098af8fe9674f66b1b81f4
ms.sourcegitcommit: fbaa2ce2cfb4d56d8c4cf2fa2d95489bdfcb7ff0
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/30/2020
ms.locfileid: "43947907"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Exchange Online PowerShell mikro aiztures vai ierobežošana

Palaižot skriptus vai komandlietotnes Exchange Online, jums var tikt parādīts paziņojums “Piemērotas mikro aiztures” vai piemērota ierobežošana. Tālāk ir sniegti divi ieteikumi par to:

- Iespējams, ka vēlaties izmēģināt [Exchange Online v2 PowerShell moduli](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), kas iekļauj komandlietotnes, kas ir balstītas uz REST API un tām ir būtiski lielāka veiktspēja. Šis varētu būt lielisks risinājums daudzām bieži izmantotām Get- komandlietotnēm.
- Ja jums ir jāizmanto komandlietotnes, kas vēl nav iekļautas v2 modulī, lūdzu, lasiet [PowerShell komandlietotņu palaišana lielam Office 365 lietotāju skaitam](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), kur ir aprakstīts risinājums PowerShell ierobežojumu apiešanai pakalpojumā Exchange Online.
