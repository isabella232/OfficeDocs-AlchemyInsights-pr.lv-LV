---
title: Krāpšanas drošības padoms pārbaužu datu problēmu novēršana
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: c7ee1fcc887a3221b5f2acda1aa6ae6beb03cb96686d4ecb7828a02f8ff48302
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955973"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Krāpšanas drošības padoms pārbaužu datu problēmu novēršana

Ja saņemat ziņojumu drošības padoms kurā teikts "Sūtītājs neizdevās veikt krāpšanas noteikšanu, bet var nebūt tas, kas izskatās kā", sūtītājam neizdevās nodot DKIM vai SPF autentifikācijas pārbaudes. Vislabākais veids, kā šo problēmu atrisināt, ir atļaut sūtītājam sevi autorizēt. Ja sūtītājs sūta ziņojumu jūsu vārdā, jums tie ir jāpilnvaro, pievienojot sūtītāja IP adresi savam SPF ierakstam.
  
[Papildinformāciju skatiet rakstā Sarkanā (aizdomīgā)](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) drošības padoms, kurā tiek meklētas krāpšanas atklāšanas pārbaudes.
  
Lūk, dažas citas saites, kas var palīdzēt:
  
- [Kā Microsoft izmanto sūtītāja politikas struktūru (SPF), lai novērstu izlikšanās](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [SPF iestatīšana, lai palīdzētu novērst izlikšanās](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
