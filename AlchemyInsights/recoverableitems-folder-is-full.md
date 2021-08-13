---
title: 1336 mape Atkopjamie vienumu vienumi ir pilna
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 5c8d53ceabf2428f3d6d765040f1b789b6bbeda04a22dd7fde0d2d728fd17d93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061763"
---
# <a name="the-recoverable-items-folder-is-full"></a>Mape Atkopjamie vienumi ir pilna

Pastkastu Exchange Online noklusējuma krātuves ierobežojums atkopjamo vienumu mapei ir 30 GB. Mapes Atkopjamie vienumi krātuves ierobežojums tiek automātiski palielināts līdz 100 GB, ja pastkaste tiek aizturēta saistībā ar tiesas procesu, e-datu atklāšanas aizturēšanu vai tiek piešķirta saglabāšanas politika.

Ja mape Atkopjamie vienumi sasniedz krātuves ierobežojumu, pastkastes funkcionalitāte tiek ietekmēta šādos veidos:

- Lietotājs nevar izdzēst vienumus no pastkastes.

- Pārvaldīto mapju palīgs nevar izdzēst vienumus, ņemot vērā saglabāšanas atzīmi vai pārvaldītos mapes iestatījumus.

- Pastkastēs, kurās ir iespējota atsevišķa vienuma atkopšana vai kuras ir aizturētas, kopēšanas un rakstīšanas lapas aizsardzības process nevar uzturēt lietotāja rediģēto vienumu versijas.

- Pastkastēm, kurās ir iespējota pastkastes audita reģistrēšana, mapes Atkopjamie vienumi apakšmapē Auditi nevar saglabāt pastkastes audita žurnāla ierakstus.

Pastkastēm, kuras nav aizturētas, administratori var izmantot PowerShell komandu, Exchange Online PowerShell, lai izdzēstu vienumus mapē `Search-Mailbox -SearchDumpsterOnly -DeleteContent` Atkopjamie vienumi. Papildinformāciju skatiet tālāk sniegtajās tēmās.

- [Ziņojumu meklēšana un dzēšana](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Pastkastēm, kas ir aizturētas, administratoriem ir jānoņem aizturēšana, lai viņi varētu izdzēst vienumus no mapes Atkopjamie vienumi. Papildinformāciju skatiet [rakstā Vienumu dzēšana mākonī bāzētu pastkastu mapē Atkopjamie vienumi, ja tās ir aizturētas.](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)

Lai neļautu mapes Atkopjamie vienumi kļūt pilnai, administratori var palielināt aizturēto pastkastu mapes Atkopjamie vienumi krātuves ierobežojumu un iestatīt pastkastes saglabāšanas politiku, kas pārvieto vienumus no mapes Atkopjamie vienumi uz lietotāja arhīva pastkasti. Skatiet [sadaļu Aizturēto pastkastu atkopjamo vienumu kvotas palielināšana.](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold)
