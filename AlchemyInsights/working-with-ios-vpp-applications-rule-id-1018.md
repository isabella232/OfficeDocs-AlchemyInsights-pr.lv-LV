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
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688953"
---
# <a name="working-with-ios-vpp-applications"></a>Darbs ar iOS VPP lietojumprogrammām

Izlasiet, [kā pārvaldīt iOS lietojumprogrammas, kas iegādātas, izmantojot lielapjoma pirkumu programmu, ar Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) , lai iegūtu informāciju par līdzekļiem, ierobežojumiem un darbībām, kas jāveic, lai izmantotu Apple lielapjoma pirkumu programmu un tās atbalstu pakalpojumā Microsoft Intune.
  
 **Biežāk sastopamās problēmas:** "Esmu piešķīris iOS VPP lietojumprogrammu saviem lietotājiem, taču instalēšana neizdevās."
  
- Tas var notikt, ja vairāku mobilo ierīču pārvaldības pakalpojumu sniedzēji izmanto vienu VPP žetonu. VPP žetoni no Apple var tikt izmantoti tikai ar vienu pakalpojumu sniedzēju. Ja izmantojāt VPP zīmi ar vairākiem pakalpojumu sniedzējiem, jums ir atkārtoti jāaugšupielādē pilnvara Intune.

- Instalēšana var neizdoties arī tad, ja instalācijas kopējais skaits pārsniedz licenču skaitu. Lai skatītu licenču lietojuma pārskatu, dodieties uz lapu **Intune Mobile Apps** \> **lietojumprogrammu licences** . Lai uzzinātu, kā atgūt licences izmantošanai, skatiet [šo rakstu.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
