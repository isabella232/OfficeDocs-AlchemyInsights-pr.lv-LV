---
title: Office izvietošanas rīka izmantošana
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 39a011d4b121492d222ff620e70d9860231b7bcfe0d7fd2ecfd93de1ef502f5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083777"
---
# <a name="using-the-office-deployment-tool-odt"></a>Office izvietošanas rīka (ODT) izmantošana

Varat izmantot Office rīku (ODT), lai izvietotu Office 365 versijas Office. Office rīks (setup.exe) tiek palaists no komandrindas un izmanto XML konfigurācijas failu, lai noteiktu, kādi iestatījumi ir jālieto, izvietojot Office.
  
1. Lejupielādējiet jaunāko Office izvietošanas rīku no [Microsoft lejupielādes centra.](https://go.microsoft.com/fwlink/p/?LinkID=626065)

2. Izmantojiet Office [rīku (OCT), lai](https://config.office.com) atlasītu izvietošanas preferences un izveidotu xml faila konfigurāciju. Eksportējiet konfigurācijas failu un ievietojiet to lokāli tajā pašā mapē, setup.exe atrodas.

    **Piezīme.** Office instalēšanas problēmas parasti rodas nepareizi konfigurētu vai malformatētu konfigurācijas failu dēļ. Lai novērstu šādas problēmas, iesakām izmantot pielāgošanas rīku Office lai izveidotu konfigurācijas failu. Varat arī importēt esošos konfigurācijas failus Office pielāgošanas rīkā.

3. Priviliģētā komandu uzvednē pārslēdzieties uz atrašanās vietu, setup.exe atrodas un palaidiet Office izvietošanas rīku lejupielādes režīmā un norādiet tikko saglabāto konfigurācijas failu. Šajā piemērā konfigurācijas faila nosaukums ir Configuration.xml:

```setup.exe /download Configuration.xml```

4.Palaidiet Office izvietošanas rīku konfigurēšanas režīmā un norādiet konfigurācijas failu.

```setup.exe /configure Configuration.xml```

**Piezīme.** Šī darbība ir jāveic klienta datorā, kurā vēlaties instalēt Office un jābūt lokālā administratora atļaujām šajā datorā.

Papildinformāciju par Office izvietošanas rīka izmantošanu Microsoft 365 programmas lieluzņēmumiem izvietošanas scenārijos, skatiet [rakstā Office izvietošanas rīka pārskats.](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool) Papildinformāciju par pielāgošanas Office izmantošanu skatiet rakstā Pārskats [Office pielāgošanas rīku.](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)
