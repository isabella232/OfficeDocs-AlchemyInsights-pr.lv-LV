---
title: Izmantojot rīku Office izvietošanai
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 874bb7883bca4f062e85963a6828a771cd2dad9b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/22/2019
ms.locfileid: "36531582"
---
# <a name="using-the-office-deployment-tool-odt"></a>Izmantojot Office izvietošanas rīku (ODT)

Izmantojat Office izvietošanas rīku (ODT) izvietot Office 365 Office versijām. Office ieviešanas rīks (setup.exe) tiek palaista no komandrindas un konfigurācijas XML failu izmanto, lai noteiktu, kādus iestatījumus lietot, izvietojot Office.
  
1. Lejupielādēt jaunāko versiju Office izvietošanas rīku no [Microsoft lejupielādes centra](http://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Izmantojiet [Office pielāgošanas rīks (AZT)](https://config.office.com) atlasiet izvietošanas preferences un izveidot konfigurācijas XML failu. Konfigurācijas faila eksportēšanas un lokāli novietot tajā pašā mapē, kur atrodas setup.exe.

    **Piezīme:** Office instalācijas, bieži rodas problēmas sakarā ar misconfigured vai malformatted konfigurācijas failus. Lai izvairītos no šādas problēmas, ieteicams izmantot Office pielāgošanas rīku, lai izveidotu konfigurācijas failu. Esošās konfigurācijas failus var arī importēt Office pielāgošanas rīks.

3. Paaugstinātu komandu uzvednes, pāriet uz vietu, kur dzīvo setup.exe un palaist Office izvietošanas rīku lejupielādes režīmā un norādiet konfigurācijas failu, kuru tikko saglabājāt. Šajā piemērā konfigurācijas fails tiek nosaukts Configuration:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Palaidiet Office izvietošanas rīku konfigurēt režīmu un norādiet konfigurācijas failu.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Piezīme:** Jāpalaiž šis solis no klienta datorā, kurā vēlaties instalēt Office un jums jābūt lokālā administratora atļaujām šajā datorā.

Lai uzzinātu vairāk par Office izvietošanas rīku izmantošana Office 365 ProPlus izvietošanas scenārijos, skatiet [Office izvietošanas rīku apskats](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Sīkāku informāciju par to, kā izmantot Office pielāgošanas rīku, skatiet [Office pielāgošanas rīku apskats](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
