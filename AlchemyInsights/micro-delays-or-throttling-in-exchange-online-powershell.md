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
ms.openlocfilehash: 680df9e6e2404ff6b60b17d6ac88e202e9a7bb25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830040"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Exchange Online PowerShell mikro aiztures vai ierobežošana

Palaižot skriptus vai komandlietotnes Exchange Online, jums var tikt parādīts paziņojums “Piemērotas mikro aiztures” vai piemērota ierobežošana. Tālāk ir sniegti divi ieteikumi par to:

- Iespējams, ka vēlaties izmēģināt [Exchange Online v2 PowerShell moduli](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), kas iekļauj komandlietotnes, kas ir balstītas uz REST API un tām ir būtiski lielāka veiktspēja. Šis varētu būt lielisks risinājums daudzām bieži izmantotām Get- komandlietotnēm.
- Ja jums ir jāizmanto komandlietotnes, kas vēl nav iekļautas v2 modulī, lūdzu, lasiet [PowerShell komandlietotņu palaišana lielam Office 365 lietotāju skaitam](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), kur ir aprakstīts risinājums PowerShell ierobežojumu apiešanai pakalpojumā Exchange Online.
