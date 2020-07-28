---
title: Intune ierīces noliktava
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439657"
---
# <a name="intune-device-inventory"></a>Intune ierīces noliktava

Ierīču asmens sniedz administratora ieskatu par ierīcēm, kas ir iekļautas pārvaldības Intune ierīcē katrai ierīcei. Parādītajā informācijā ietilpst: aparatūra, atklātās lietojumprogrammas, ierīces atbilstības stāvoklis un ierīces konfigurācijas stāvoklis.

Aparatūras un atklāto lietojumprogrammu inventarizācijas dati tiek apkopoti septiņu dienu ciklā. Ziņotās aparatūras lietojumprogrammas un īpašie elementi atšķiras atkarībā no ierīces operētājsistēmas un tā, vai ierīce ir personiski vai uzņēmuma īpašumā.

Papildinformāciju skatiet rakstā [ierīces datu skatīšana Intune](https://docs.microsoft.com/intune/device-inventory).

**BUJ**

Jautājums: Es nesaņemu pilnu sarakstu ar lietojumprogrammām, kas ir iekļautas Intune Windows ierīcēs. kāpēc ne?

A: šajā laikā ir norādītas tikai modernās lietojumprogrammas, kas paredzētas Windows 10 datoriem, kas ir identificēti kā korporatīvās ierīces. Intune neapkopo informāciju par šajās ierīcēs instalētajām Win32 programmām.

J: Kāpēc tālruņu numuri nav apkopoti no visām ierīcēm?

A: tālruņi, kas iedalīti kā korporatīvās ierīces pakalpojumā Intune, netiek identificēti ar pilnu tālruņa numuru, piemēram, varat izpildīt mobilo ierīču inventarizācijas atskaiti. No jūsu ierīces tālruņa numuri vienmēr tiek daļēji maskēti ar zvaigznītēm (* * * * *) un tiek parādīti tikai pēdējie četri cipari.