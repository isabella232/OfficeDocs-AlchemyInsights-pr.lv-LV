---
title: Novecojušu ierīču automātiska tīrīšana sistēmā Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555223"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a>Novecojušu ierīču automātiska tīrīšana sistēmā Intune

Intune sniedz administratoram iespēju konfigurēt laika intervālu starp 90 un 270 dienām, pēc kura sasmacis ierīces tiek noņemtas no pakalpojuma. Šis iestatījums ir organizācijas mērogs, un pēc tam, kad tā ir aktivizēta, ir spēkā nekavējoties. Visas ierīces, kuras nav pārbaudījušas Intune serverī uz periodu, kas pārsniedz iestatījumu, tiek neatgriezeniski izdzēstas.

**Piezīmes** Šī tīrīšanas darbība atbilst tikai MDM ierīces objektiem. Tikai EAS ierīces objekti tiek izslēgti.

Lai iegūtu papildinformāciju par to, kad ierīce ir piemērota dzēšanai, ņemot vērā ierīces tīrīšanas iestatījumu un tās "stāvokli":

Iestatījums: **izdzēsiet ierīces pēc pēdējā atdošanas datuma: Jā (zināma vērtība (N) noteiktās dienās)**

- Atkarībā no parametra Value (N), Intune pakalpojums izdzēš ierīci norādītajās dienās pēc tam, kad tā pēdējoreiz ir veiksmīgi pārbaudīta.

Iestatījums: **pēc pēdējā atdošanas datuma dzēst ierīces: Nē**

- 180 dienas pēc tam, kad ierīces sertifikāts ir beidzies un nav atjaunots, ierīce tiek izdzēsta.

**Piezīmes** Abos gadījumos ierīce ir veiksmīgi reģistrēta Intune. Reģistrācija notiek pirmās ierīces atdošanas laikā ar Intune pakalpojumu.

Ja ierīce veiksmīgi piesakās Intune, bet nekļūst par Intune reģistrēto, šī ierīce tiek izdzēsta 270 dienās pēc reģistrācijas. (90 dienas, lai atzīmētu ierīci kā atsauktu, un pēc tam vēl 180 dienas, lai dzēstu ierakstu.)

Šobrīd Intune konsolē nepastāv mehānisms, lai noteiktu ierīces sertificēšanas derīguma termiņu katrai ierīcei.