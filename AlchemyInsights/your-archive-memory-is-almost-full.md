---
title: Jūsu arhīva pastkaste ir gandrīz pilna
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 085d9b211d5a8e9a0e1eb12af14d87a4e59c844a3afa012095dfd60db316ad14
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046759"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Jūsu arhīva pastkaste ir gandrīz pilna

Ja lietotājs saņem brīdinājumu; **Jūsu arhīva pastkaste ir gandrīz** pilna vai jāpalielina arhīva pastkaste, lūk, daži padomi:

1. Ja lietotājam ir piešķirta Exchange Online 1. plāns, jauniniet uz **Exchange Online 2.** plāna licenci, lai palielinātu to lielumu no 50 GB līdz 100 GB.
1. Ja lietotājam jau ir piešķirts kāds no šiem: **Exchange Online 2.** plāns vai Exchange Online 1. plāns ar Exchange Online arhivēšana pievienojumprogrammu, veiciet tālāk norādītās darbības, lai iespējotu automātiskās izvēršanas arhivēšanu:.
 
    1. [Savienošana uz Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    2. Palaidiet lietotājam šādu komandsīklietotni:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Palaidiet šādu komandsīklietotni, lai pārliecinātos, vai tas ir iespējots lietotājam:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Papildinformāciju skatiet rakstā:

- [Neierobežota arhivēšanas iespējošana — administrēšanas palīdzība — Microsoft 365 atbilstības | Microsoft dokumenti](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Online ierobežojumi — pakalpojumu apraksti | Microsoft dokumenti](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Jaunināšana uz citu biznesa plāna | Microsoft dokumenti](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

