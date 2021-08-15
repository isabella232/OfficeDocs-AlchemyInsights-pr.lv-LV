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
ms.openlocfilehash: ef06cfe41eee5d67bf82d4f64875ddafac82ee2062aade761f81b906cd428dd5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54024213"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>Kā iestatīt vairākfunkciju ierīci vai programmu e-pasta nosūtīšanai

Lai iegūtu informāciju par iespējām un norādījumiem, skatiet rakstu [Kā iestatīt vairākfunkciju ierīci vai programmu e-pasta nosūtīšanai, izmantojot Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).
  
Ja jums ir ierīce vai lietojumprogramma, kas nesen pārtrauca darboties, visbiežāk sastopamās problēmas ir:

- **Ar autentifikāciju saistītas kļūdas, izmantojot SMTP autentifikācijas klienta iesniegšanu** Nesen veicām dažas izmaiņas saistībā ar SMTP autentifikācijas darbību. Papildinformāciju par to, kā novērst problēmas, skatiet sadaļā To printeru, skeneru un LOB lietojumprogrammu problēmu [novēršana,](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)kas nosūta e-pastu, izmantojot Microsoft 365 vai Office 365 .
- **Mēs pieņemam tikai TLS 1.2 versiju, kamēr** tiek izveidots drošs savienojums ar Office 365 Ja izmantojat drošo savienojumu (TLS), pārliecinieties, vai jūsu lietojumprogrammas ierīce atbalsta TLS 1.2. Papildinformāciju skatiet rakstā [Gatavošanās TLS 1.2 sagatavošanai programmā Office 365 un Office 365 GCC.](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)
 
Informāciju par citām problēmām un risinājumiem skatiet rakstā To printeru, skeneru un LOB lietojumprogrammu problēmu novēršana, kas sūta [e-pastu, Microsoft 365 vai Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).

Lai redzētu ietekmētās ierīces, dodieties uz [SMTP Auth klientu atskaiti](https://protection.office.com/mailflow/dashboard).

**Piezīme.** Exchange Online nav pielāgoti lielapjoma pasta sūtīšanas scenāriji. Lai nosūtītu komercpasta lielapjoma ziņojumus (piemēram, klientu biļetenus), izmantojiet trešo pušu pakalpojumu sniedzējus, kas specializējas šajos pakalpojumos.
