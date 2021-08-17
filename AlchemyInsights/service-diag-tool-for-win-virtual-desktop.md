---
title: Pakalpojumu diagnostikas rīks Windows virtuālajai darbvirsmai
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: 58688e3216ba6777b1a4f76095bd39c81a2d2a8294e06b6bc61c7134f6d589f9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052393"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Pakalpojumu diagnostikas rīks Windows virtuālajai darbvirsmai

Windows Virtuālā darbvirsma (Virtual Desktop – WVD) piedāvā diagnostikas rīku, kas administratoriem ļauj identificēt kļūdas, izmantojot vienu interfeisu. Šis rīks reģistrē ar diagnostiku saistītu informāciju ikreiz, kad WVD izmanto kāds lietotājs, kuram piešķirta WVD loma. Katrā žurnālā ir iekļauta informācija par darbībā iesaistīto WVD lomu, sesijas laikā parādītajiem kļūdu ziņojumiem un informāciju par nomnieku un lietotāju. Azure Log Analytics var konfigurēt, lai tvertu diagnostikas rīka izveidoto darbību žurnālu. Tālāk aprakstīts, kā to paveikt.

1. Izveidojiet Log Analytics darbvietu [Azure portālā vai](https://go.microsoft.com/fwlink/?linkid=2129500) [pakalpojumā Azure PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)
1. [Savienošana Windows datorus azure monitorā](https://go.microsoft.com/fwlink/?linkid=2129913). Iegūstiet darbvietas ID un darbvietas primāro atslēgu. Iestatīšanas vednim ir nepieciešama šī informācija, lai pareizi konfigurētu aģentu un nodrošinātu, ka tas var sazināties ar Azure Monitor.
1. [Pašpiegādes diagnostika datus uz jūsu darbvietu.](https://go.microsoft.com/fwlink/?linkid=2128284) Varat pašpiegādes diagnostikas datus no sava WVD nomnieka uz darbvietas žurnālu analīzi.
1. [Identificējiet un diagnosticējiet](https://go.microsoft.com/fwlink/?linkid=2128338) problēmas, kas ir iekšējas vai ārējas attiecībā pret WVD.

Lai uzzinātu vairāk par pakalpojumu diagnostikas rīka konfigurēšanu WVD, skatiet rakstu Log [Analytics izmantošana diagnostikas līdzeklim.](https://go.microsoft.com/fwlink/?linkid=2128084)
