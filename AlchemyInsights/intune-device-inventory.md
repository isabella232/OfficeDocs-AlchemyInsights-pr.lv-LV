---
title: Intune ierīces noliktava
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667885"
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