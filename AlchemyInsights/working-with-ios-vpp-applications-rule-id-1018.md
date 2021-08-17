---
title: Darbs ar iOS VPP lietojumprogrammu kārtulas ID 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: f693d12ff0f9c193cba0c6a6802b22d7acd37532c65986e5f6613e18c021f06b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083021"
---
# <a name="working-with-ios-vpp-applications"></a>Darbs ar iOS VPP lietojumprogrammām

Izlasiet rakstu Kā pārvaldīt iOS programmas, kas iegādātas, izmantojot lielapjoma iegādes programmu, izmantojot [Microsoft Intune,](https://docs.microsoft.com/intune/vpp-apps-ios) lai uzzinātu par līdzekļiem, ierobežojumiem un darbībām, kas jāveic Apple lielapjoma iegādes programmā, kā arī par tās atbalstu Microsoft Intune.
  
 **Bieži sastopamās problēmas.** "I assigned an iOS VPP app to my users, but the installation failed." (I piešķīris iOS VPP programmu saviem lietotājiem, bet instalēšana neizdevās.)
  
- Tā var notikt, ja viens VPP marķieris tiek izmantots vairākiem mobilo ierīču pārvaldības pakalpojumu sniedzējiem. VPP marķierus no Apple var izmantot tikai kopā ar vienu pakalpojumu sniedzēju. Ja izmantojāt VPP marķieri ar vairākiem pakalpojumu sniedzējiem, marķieris ir atkārtoti jāielādē Intune.

- Instalēšana var neizdoties arī tad, ja kopējais instalāciju skaits pārsniedz licenču skaitu. Lai skatītu licenču lietojuma atskaiti, dodieties uz **Intune mobilo programmu** \> **programmu licenču** lapu. Informāciju par to, kā atgūt licences, kas tiek lietotas, [skatiet šajā rakstā.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
