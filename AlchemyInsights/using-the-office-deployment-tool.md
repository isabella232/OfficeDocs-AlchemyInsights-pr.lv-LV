---
title: Izmantojot Office izvietošanas rīku
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: d941bce524dc797d5dcbb7213bded6919fd01b7d
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010874"
---
# <a name="using-the-office-deployment-tool-odt"></a>Izmantojot Office izvietošanas rīku (ODT)

Office izvietošanas rīks (ODT) izmanto, lai izvietotu Office 365 Office versijas. Office izvietošanas rīks (setup. exe) tiek palaists no komandrindas un izmanto konfigurācijas XML failu, lai noteiktu, kādi iestatījumi jālieto, izvietojot Office.
  
1. Lejupielādējiet Office izvietošanas rīka jaunāko versiju no [Microsoft lejupielādes centra](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Izmantojiet [Office pielāgošanas rīku (Oct)](https://config.office.com) , lai atlasītu izvietošanas preferences un izveidotu konfigurācijas XML failu. Eksportējiet konfigurācijas failu un novietojiet to lokāli tajā pašā mapē, kur atrodas setup. exe.

    **Piezīme:** Office instalācijas problēmas parasti rodas nepareizas konfigurēšanas vai nepareizi formatētu konfigurācijas failu dēļ. Lai izvairītos no šādām problēmām, ieteicams izmantot Office pielāgošanas rīku, lai izveidotu konfigurācijas failu. Varat arī importēt esošos konfigurācijas failus Office pielāgošanas rīkā.

3. Priviliģētā komandu uzvednē pārslēdzieties uz vietu, kur atrodas setup. exe, un palaidiet rīku Office Deployment lejupielādes režīmā un norādiet tikko saglabāto konfigurācijas failu. Šajā piemērā konfigurācijas faila nosaukums ir Configuration. XML:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Palaidiet rīku Office izvietošanas konfigurēšana režīmā un norādiet konfigurācijas failu.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Piezīme:** Šī darbība ir jāpalaiž klienta datorā, kurā vēlaties instalēt Office, un jums ir jābūt lokālā administratora atļaujām šajā datorā.

Lai uzzinātu vairāk par Office izvietošanas rīka lietošanu Microsoft 365 lietojumprogrammām uzņēmuma izvietošanas scenārijiem, skatiet [pārskats par Office izvietošanas rīku](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Plašāku informāciju par to, kā izmantot Office pielāgošanas rīku, skatiet sadaļā [pārskats par Office pielāgošanas rīku](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
