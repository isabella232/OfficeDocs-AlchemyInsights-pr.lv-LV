---
title: Microsoft Edge atbalsts Microsoft Defender lietojumprogrammu aizsargam
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583580"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a>Microsoft Edge atbalsts Microsoft Defender lietojumprogrammu aizsargam

Paredzēts darbam ar Windows 10 un Microsoft Edge, lietojumprogramma Guard izmanto aparatūras izolēšanas pieeju, kas ļauj lietotājam pāriet uz neuzticamu vietni, izmantojot izolētu, Hyper-V-iespējoto konteineru, kas atdalīts no resursdatora.

Uzņēmuma administrators definē uzticamo tīmekļa vietņu, mākoņa resursu un iekšējo tīklu sarakstu. Kad lietotājs apmeklē vietni, kas nav sarakstā, Microsoft Edge atvērs šo vietni konteinerā. Tas nozīmē, ka, ja vietne izrādās ļaunprātīga, resursdatora dators paliks aizsargāts, un uzbrucējs neredzēs uzņēmuma datus.

Tiek atbalstīta paplašinājumu instalēšana konteinerā Microsoft Edge versija 81, un to var kontrolēt, izmantojot politiku. UpdateURL adrese, kas tiek izmantota ExtensionInstallForcelist politikā, ir jāpievieno kā neitrāls resurss tīkla izolācijas politikās, ko izmanto lietojumprogrammas aizsargs.

Papildinformāciju skatiet rakstā [Microsoft Edge atbalsts Microsoft Defender lietojumprogrammu aizsargam](https://go.microsoft.com/fwlink/?linkid=2134229).
