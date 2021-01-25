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
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974407"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Jūsu arhīva pastkaste ir gandrīz pilna

Ja lietotājs saņem brīdinājumu; **Jūsu arhīva pastkaste ir gandrīz pilna** vai ir jāpalielina savas arhīva pastkastes lielums, šeit sniegti daži padomi.

1. Ja lietotājam ir piešķirts Exchange Online 1. plāns, jauniniet uz **Exchange Online 2. plānu** , lai palielinātu lielumu no 50 GB līdz 100gb.
1. Ja lietotājam jau ir piešķirts kāds no šiem: **Exchange Online 2. plāns** vai Exchange Online 1. plāns ar Exchange Online arhivēšanas pievienojumprogrammu, veiciet tālāk norādītās darbības, lai iespējotu automātisko arhivēšanu.
 
    1. [Savienojuma izveide ar Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    2. Palaidiet tālāk norādīto unifiedgroup lietotājam.  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Palaidiet tālāk norādīto unifiedgroup, lai pārliecinātos, vai tas ir iespējots lietotājam.  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Papildinformāciju skatiet rakstā:

- [ Iespējot neierobežotu arhivēšanu — administrēšanas palīdzība — Microsoft 365 atbilstība | Microsoft dokumenti](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Online ierobežojumi — pakalpojumu apraksti | Microsoft dokumenti](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Jaunināšana uz citu biznesa plānu | Microsoft dokumenti](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

