---
title: Drošības padoma novēršana krāpšanas atklāšanas pārbaužu gadījumā
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
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834738"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Drošības padoma novēršana krāpšanas atklāšanas pārbaužu gadījumā

Ja saņemat drošības padomu, kas vēsta "Sūtītājs neizdevās veikt krāpšanas atklāšanas pārbaudes un var nebūt tas, kas izskatās pēc", sūtītājam neizdevās nodot DKIM vai SPF autentifikācijas pārbaudes. Vislabākais veids, kā šo problēmu atrisināt, ir atļaut sūtītājam sevi autorizēt. Ja sūtītājs sūta ziņojumu jūsu vārdā, jums tie ir jāpilnvaro, pievienojot sūtītāja IP adresi savam SPF ierakstam.
  
[Papildinformāciju skatiet rakstā Sarkanā (aizdomīgā)](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) drošības padoma problēmu novēršana attiecībā uz krāpšanas noteikšanu.
  
Lūk, dažas citas saites, kas var palīdzēt:
  
- [Kā Microsoft izmanto sūtītāja politikas struktūru (SPF), lai novērstu izlikšanās](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [SPF iestatīšana, lai palīdzētu novērst izlikšanās](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
