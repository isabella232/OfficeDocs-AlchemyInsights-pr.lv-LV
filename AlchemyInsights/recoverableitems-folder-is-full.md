---
title: 1336 RecoverableItems mape ir pilna
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 05e7b47a2200c3b0500e7d786166966ea301179a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/28/2019
ms.locfileid: "35370394"
---
# <a name="the-recoverable-items-folder-is-full"></a>Atkopt vienumus mape ir pilna

Exchange Online pastkastēm Office 365, atkopt vienumus mapē noklusējuma glabāšanas limits ir 30 GB. Atkopt vienumus mapē krātuves ierobežojums automātiski palielina līdz 100GB ja pastkaste tiek likts uz tiesāšanos turiet eDiscovery aizturēšana, vai ir piešķirta biroja 365 saglabāšanas politiku.

Atkopt vienumus mapē sasniedz krātuves limits, funkcionalitāti pastkastes tiek ietekmētas šādos veidos:

- Lietotājs nevar dzēst vienumus no pastkastes.

- Pārvaldītas mapes palīgu nevar dzēst vienumus, pamatojoties uz aiztures tag vai pārvaldītās mapes iestatījumus.

- Pastkastēm ir iespējota vienotā vienumu atkopšana vai tiek aizturēta, lapas kopiju rakstīšanas aizsardzības procesā nevar uzturēt elementu rediģēt lietotājs versijām.

- Pastkastēm, kuriem ir pastkaste, audita iespējotu reģistrēšanu, pastkastes audita žurnāla ieraksti var tikt saglabāti revīziju apakšmapei mapē atkopt vienumus.

Pastkastēm, kas nav aizturēts, varat izmantot admins `Search-Mailbox -SearchDumpsterOnly -DeleteContent` komandu Exchange Online PowerShell, lai izdzēstu vienumus atkopt vienumu mapē. Papildinformāciju skatiet tālāk sniegtajās tēmās.

- [Meklēt un dzēst ziņojumus](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [Meklēšanas pastkasti](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Pastkastes, kas ir aizturēta, admins ir noņemt aizturēšanu, pirms tie var atkopt vienumus mapē Izdzēstie vienumi. Plašāku informāciju skatiet [Dzēst vienumus atgūstamo vienumus, turiet mākonis balstītu pastkastītes uz mapi](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Lai nekļūtu atkopt vienumus mapē pilna, admins var palielināt krātuves ierobežojums atgūstamo vienumus mapē pastkastēm, turēt un iestatīt pastkasti saglabāšanas politika, kas pārvieto vienumus no mapes atkopt vienumus lietotāja Arhīvs pastkasti. Sk. [palielināt atgūstamo vienumus pastkastes uz kvotu turiet](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
