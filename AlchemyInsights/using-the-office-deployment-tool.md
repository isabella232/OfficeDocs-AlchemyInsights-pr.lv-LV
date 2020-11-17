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
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085839"
---
# <a name="using-the-office-deployment-tool-odt"></a>Izmantojot Office izvietošanas rīku (ODT)

Izmantojiet Office izvietošanas rīku (ODT), lai izvietotu Office 365 Office versijas. Office izvietošanas rīku (setupodt.exe) izpilda no komandrindas un izmanto konfigurācijas XML failu, lai noteiktu, kādi iestatījumi jālieto, izvietojot Office.
  
1. Lejupielādējiet jaunāko Office izvietošanas rīka versiju no [Microsoft lejupielādes centra](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Izmantojiet [Office pielāgošanas rīku (Oct)](https://config.office.com) , lai atlasītu izvietošanas preferences un izveidotu konfigurācijas XML failu. Eksportējiet konfigurācijas failu un novietojiet to lokāli tajā pašā mapē, kur atrodas setupodt.exe.

    **Piezīme:** Office instalēšanas problēmas parasti rodas nepareizi konfigurētu vai malformatted konfigurācijas failu dēļ. Lai izvairītos no šādām problēmām, iesakām izmantot Office pielāgošanas rīku, lai izveidotu konfigurācijas failu. Varat arī importēt esošos konfigurācijas failus Office pielāgošanas rīkā.

3. Priviliģētā komandu uzvednē pārejiet uz atrašanās vietu, kur setupodt.exe atrodas, un palaidiet Office izvietošanas rīku lejupielādes režīmā un norādiet konfigurācijas failu, kuru tikko saglabājāt. Šajā piemērā konfigurācijas faila nosaukums ir Configuration.xml:

```setupodt.exe /download Configuration.xml```

4. palaidiet Office izvietošanas rīku konfigurēšanas režīmā un norādiet konfigurācijas failu.

```setupodt.exe /configure Configuration.xml```

**Piezīme:** Šī darbība ir jāveic no klienta datora, kurā vēlaties instalēt Office, un jums ir nepieciešamas lokālā administratora atļaujas šajā datorā.

Lai uzzinātu vairāk par to, kā izmantot Office izvietošanas rīku Microsoft 365 lietojumprogrammām uzņēmuma izvietošanas scenārijiem, skatiet rakstu [pārskats par Office izvietošanas rīku](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Lai iegūtu papildinformāciju par to, kā izmantot Office pielāgošanas rīku, skatiet rakstu [pārskats par Office pielāgošanas rīku](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
