---
title: Pakalpojuma diagnostikas rīks Windows virtuālajai darbvirsmai
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
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/14/2020
ms.locfileid: "49678624"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Pakalpojuma diagnostikas rīks Windows virtuālajai darbvirsmai

Windows virtuālā darbvirsma (WVD) piedāvā diagnostikas rīku, kas administratoriem ļauj noteikt kļūdas, izmantojot vienu interfeisu. Šis rīks reģistrē diagnostiku ar diagnostikas informāciju, kad WVD izmanto kāds, kam ir piešķirta WVD loma. Katrā žurnālfailā ir iekļauta informācija par aktivitāti iesaistīto WVD lomu, kļūdu ziņojumi, kas tiek parādīti sesijas laikā, kā arī informācija par nomnieku un lietotāju. Azure LG Analytics var konfigurēt, lai tvertu diagnostikas rīka izveidoto darbību žurnālu. Tālāk aprakstīts, kā to paveikt.

1. Izveidojiet žurnālu analīzes darbvietu ar [Azure portālu](https://go.microsoft.com/fwlink/?linkid=2129500) vai [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).
1. [Windows datoru savienošana ar Azure monitoru](https://go.microsoft.com/fwlink/?linkid=2129913). Iegūstiet darbvietas ID un darbvietas primāro atslēgu. Iestatīšanas vednim ir nepieciešama šī informācija, lai pareizi konfigurētu aģentu un nodrošinātu, ka tas var sazināties ar Azure monitoru.
1. [Stumiet diagnostikas datus darbvietā](https://go.microsoft.com/fwlink/?linkid=2128284). Varat push diagnostikas datus no sava WVD nomnieka uz savas darbvietas žurnālu analīzi.
1. [Identificējiet un diagnosticējiet problēmas](https://go.microsoft.com/fwlink/?linkid=2128338) , kas ir iekšējas vai ārējas saistībā ar WVD.

Lai uzzinātu vairāk par pakalpojumu diagnostikas rīka konfigurēšanu programmai WVD, skatiet rakstu [diagnostikas līdzekļa žurnālu analīzes lietošana](https://go.microsoft.com/fwlink/?linkid=2128084).
