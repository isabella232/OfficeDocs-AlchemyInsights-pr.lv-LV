---
title: E-pasta retranslēšana, izmantojot Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: f02daad7d4b4a11f8d8bb1ef1467db5809cbd291
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324369"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>Kā iestatīt vairākfunkciju ierīci vai programmu e-pasta nosūtīšanai

Lai iegūtu informāciju par iespējām un norādījumiem, skatiet rakstu [Kā iestatīt vairākfunkciju ierīci vai programmu e-pasta nosūtīšanai, izmantojot Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).
  
Ja jums ir ierīce vai lietojumprogramma, kas nesen pārtrauca darboties, visbiežāk sastopamās problēmas ir:

- **Ar autentifikāciju saistītas kļūdas, izmantojot SMTP autentifikācijas klienta iesniegšanu** Nesen veicām dažas izmaiņas saistībā ar SMTP autentifikācijas darbību. Papildinformāciju par to, kā novērst problēmas, skatiet sadaļā To printeru, skeneru un LOB lietojumprogrammu problēmu [novēršana,](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)kas sūta e-pastu, izmantojot Microsoft 365 vai Office 365 .
- **Mēs pieņemam tikai TLS 1.2 versiju, kamēr** tiek izveidots drošs savienojums ar Office 365 Ja izmantojat drošo savienojumu (TLS), pārliecinieties, vai jūsu lietojumprogrammas ierīce atbalsta TLS 1.2. Papildinformāciju skatiet rakstā [Gatavošanās TLS 1.2 sagatavošanai programmā Office 365 un Office 365 GCC.](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)
 
Informāciju par citām problēmām un risinājumiem skatiet rakstā To printeru, skeneru un LOB lietojumprogrammu problēmu novēršana, kas sūta [e-pastu, Microsoft 365 vai Office 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).

Lai redzētu ietekmētās ierīces, dodieties uz [SMTP Auth klientu atskaiti](https://protection.office.com/mailflow/dashboard).

**Piezīme.** Exchange Online nav pielāgoti lielapjoma pasta scenāriji. Lai sūtītu komercpastu vairumā (piemēram, klientu biļetenus), izmantojiet trešo pušu pakalpojumu sniedzējus, kas specializējas šajos pakalpojumos.
