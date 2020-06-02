---
title: 1336 RecoverableItems mape ir pilna
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 4f0cba480fcc05114abd8f370b84e9a37e5f2804
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510759"
---
# <a name="the-recoverable-items-folder-is-full"></a>Atkopto vienumu mape ir pilna

Exchange Online pastkastes mapes atkopt vienumus noklusējuma krātuves limits ir 30 GB. Atkopt vienumus mapē krātuves limits tiek automātiski palielināts 100 GB, ja pastkaste ir novietota aizturēšana, eDiscovery turēt vai ir piešķirta saglabāšanas politika.

Ja atkopt vienumus mapē sasniedz krātuves ierobežojums, pastkastes funkcionalitāte tiek ietekmēta šādi:

- Lietotājs nevar izdzēst vienumus no pastkastes.

- Pārvaldīto mapju palīgs nevar dzēst vienumus, pamatojoties uz saglabāšanas tagu vai pārvaldīto mapju iestatījumus.

- Pastkastēm, kas ir iespējota viena vienuma atkopšana vai tiek aizturēts, kopiju rakstīšanas lapas aizsardzības process nevar uzturēt lietotāja rediģēto vienumu versijas.

- Pastkastēm, kas ir iespējota pastkastes audita reģistrēšanu, nevar saglabāt pastkastes audita žurnāla ierakstus atkopt vienumus mapē audita apakšmapē.

Pastkastēm, kas nav aizturēts, administratori var izmantot `Search-Mailbox -SearchDumpsterOnly -DeleteContent` komandu Exchange Online PowerShell dzēst vienumus mapē atkopt vienumus. Papildinformāciju skatiet tālāk sniegtajās tēmās.

- [Ziņojumu meklēšana un dzēšana](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Meklēšanas pastkaste](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Pastkastēm, kas ir aizturēts, administratoriem ir jānoņem aizturi, pirms tie var dzēst vienumus no mapes atkopt vienumus. Lai iegūtu papildinformāciju, skatiet [vienumu dzēšana mapē atkopt vienumus mākonis balstītas pastkastes](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)aizturēts.

Lai novērstu atkopt vienumus mapē kļūst pilna, administratori var palielināt atmiņas limits atkopt vienumus mapes pastkastes aizturēts un iestatīt pastkastes saglabāšanas politika, kas pārvieto vienumus no mapes atkopt vienumus lietotāja arhīva pastkaste. Skatiet [atkopt krājumu kvota aizturētā pastkastes](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
