---
title: Pakalpojumu diagnostikas rīks Windows virtuālajai darbvirsmai
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595867"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Pakalpojumu diagnostikas rīks Windows virtuālajai darbvirsmai

Windows virtuālā darbvirsma (Windows Virtual Desktop — WVD) piedāvā diagnostikas rīku, kas administratoriem ļauj identificēt kļūdas, izmantojot vienu interfeisu. Šis rīks reģistrē ar diagnostiku saistītu informāciju ikreiz, kad WVD izmanto kāds lietotājs, kuram piešķirta WVD loma. Katrā žurnālā ir iekļauta informācija par darbībā iesaistīto WVD lomu, sesijas laikā parādītajiem kļūdu ziņojumiem un informāciju par nomnieku un lietotāju. Azure Log Analytics var konfigurēt, lai tvertu diagnostikas rīka izveidoto darbību žurnālu, izpildot šīs darbības:

1. Izveidojiet Log Analytics darbvietu [Azure portālā vai](https://go.microsoft.com/fwlink/?linkid=2129500) [pakalpojumā Azure PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)

1. [Windows datoru savienošana ar Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913). Iegūstiet darbvietas ID un darbvietas primāro atslēgu. Iestatīšanas vednim ir nepieciešama šī informācija, lai pareizi konfigurētu aģentu un nodrošinātu, ka tas var sazināties ar Azure Monitor.

1. [Pašpiegādes diagnostika datus uz jūsu darbvietu.](https://go.microsoft.com/fwlink/?linkid=2128284) Varat pašpiegādes diagnostikas datus no sava WVD nomnieka uz darbvietas žurnālu analīzi.

1. [Identificējiet un diagnosticējiet](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) problēmas, kas ir iekšējas vai ārējas attiecībā pret WVD.

Lai uzzinātu vairāk par pakalpojumu diagnostikas rīka konfigurēšanu WVD, skatiet rakstu Log Analytics izmantošana diagnostikas līdzeklim.