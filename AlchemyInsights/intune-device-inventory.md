---
title: Intune ierīču krājumi
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
ms.openlocfilehash: 00ee4f1d7130c239272e28ee8e051a18e6e0baf13040d2a892866be5900adfaf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54014079"
---
# <a name="intune-device-inventory"></a>Intune ierīču krājumi

Ierīču asmens sniedz administratoram ieskatu ierīcēs, kas tiek pārvaldības ierīcēs intune, katrai ierīcei atsevišķi. Parādītā informācija ir aparatūra, atklātas lietojumprogrammas, ierīces atbilstības stāvoklis un ierīces konfigurācijas stāvoklis.

Krājumu dati aparatūras un atklāto lietojumprogrammu krājumiem tiek apkopoti septiņu dienu ciklā. Uzrādītās lietojumprogrammas un konkrēti aparatūras elementi atšķiras atkarībā no ierīces operētājsistēmas un tā, vai ierīce pieder personiski vai korporatīvai.

Papildinformāciju skatiet rakstā [Detalizēta informācija par ierīci programmā Intune](https://docs.microsoft.com/intune/device-inventory).

**BUJ**

J: Es nesaņemu pilnu sarakstu ar programmām, kas atrodas Intune reģistrētajās Windows ierīcēs. kāpēc ne?

A. Pašlaik datoros, kas identificēti kā uzņēmuma ierīces, Windows 10 norādītas tikai modernas programmas. Intune neapkopo informāciju par šajās ierīcēs instalētajām Win32 programmām.

J: Kāpēc tālruņa numuri netiek apkopoti no visām ierīcēm?

A. Tālruņi, kas programmā Intune ir kategorizēti kā korporatīvas ierīces, netiek identificēti ar to pilno tālruņa numuru, ja, piemēram, palaižat mobilo ierīču krājumu atskaiti. Bring-you-own-device phone numbers always are partially masked with asterisks (****) and show only the last four digits.