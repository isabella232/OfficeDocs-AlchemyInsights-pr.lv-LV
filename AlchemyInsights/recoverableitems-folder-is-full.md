---
title: 1336 RecoverableItems mape ir pilna
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
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741274"
---
# <a name="the-recoverable-items-folder-is-full"></a>Mape Atkoptie vienumi ir pilna

Exchange Online pastkastēm mapes Atkoptie vienumi noklusējuma krātuves ierobežojums ir 30 GB. Mapes atkopto vienumu krātuves ierobežojums tiek automātiski palielināts līdz 100 GB, ja pastkaste tiek ievietota tiesas prāvā, e-datu atklāšanas aizturēšana vai ir piešķirta saglabāšanas politikai.

Kad mapē Atkoptie vienumi sasniedz krātuves ierobežojumu, pastkastes funkcionalitāte tiek ietekmēta tālāk norādītajos veidos.

- Lietotājs nevar izdzēst vienumus no pastkastes.

- Pārvaldītās mapes palīgs nevar izdzēst vienumus, kuru pamatā ir saglabāšanas atzīmes vai pārvaldītās mapes iestatījumi.

- Ja pastkastēm ir iespējota viena vienumu atkopšana vai tās tiek ievietotas aizturētas, kopēšanas lapu aizsardzības process nevar uzturēt lietotāja rediģēto vienumu versijas.

- Pastkastes, kurās ir iespējots pastkastes audita reģistrēšana, nav pastkastes audita žurnāla ierakstu, kurus var saglabāt mapē atlasītie vienumi.

Pastkastes, kas nav aizturētas, administratori var izmantot `Search-Mailbox -SearchDumpsterOnly -DeleteContent` komandu pakalpojumā Exchange Online PowerShell, lai dzēstu vienumus mapē Atkoptie vienumi. Papildinformāciju skatiet tālāk sniegtajās tēmās.

- [Ziņojumu meklēšana un dzēšana](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Meklēšana — pastkaste](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Pastkastēm, kas ir aizturētas, administratoriem ir jānoņem aizturēšana, pirms tie var izdzēst vienumus no mapes Atkoptie vienumi. Lai iegūtu papildinformāciju, skatiet sadaļu [vienumu dzēšana mākonī izvietoto pastkastu mapē](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Lai novērstu to, ka mape Atkoptie vienumi kļūst pilna, administratori var palielināt mapes atkopto vienumu krātuves ierobežojumu pastkastēm un iestatīt pastkastes saglabāšanas politiku, kas pārvieto vienumus no mapes Atkoptie vienumi uz lietotāja arhīva pastkasti. Skatiet tēmu [pieaugošo pastkastu kvotas palielināšana](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
