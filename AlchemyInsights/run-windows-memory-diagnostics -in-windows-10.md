---
title: Windows atmiņas diagnostikas palaišana operētājsistēmā Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/19/2020
ms.locfileid: "44357789"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Windows atmiņas diagnostikas palaišana operētājsistēmā Windows 10

Ja Windows un lietojumprogrammas datorā avarē, sasalst vai darbojas nestabilā veidā, var rasties problēmas ar datora atmiņu (RAM). Windows atmiņas diagnostiku var palaist, lai meklētu problēmas ar datora RAM.

Uzdevumjoslas meklēšanas lodziņā ierakstiet **atmiņas diagnostika**un pēc tam atlasiet **Windows atmiņas diagnostika**. 

Lai palaistu diagnostiku, DATORAM ir jārestartē. Jums ir iespēja nekavējoties restartēt (Lūdzu, saglabājiet savu darbu un aizveriet atvērtos dokumentus un e-pasta ziņojumus vispirms) vai ieplānojiet diagnostiku, lai tas tiktu palaists automātiski nākamajā datora restartēšanas reizē.

![Windows atmiņas diagnostika](media/windows-memory-diagnostic.png)

Kad dators tiek restartēts, **Windows atmiņas diagnostikas rīks** darbosies automātiski. Status un progress tiks parādīts kā diagnostika palaist, un jums ir iespēja atcelt diagnostiku, hitting **ESC** taustiņu uz klaviatūras.

Kad diagnostika ir pabeigta, sistēma Windows tiks startēta kā parasti.
Uzreiz pēc restartēšanas, kad tiek parādīta darbvirsma, tiek parādīts paziņojums (blakus **darbību centra** ikonai uzdevumjoslā), lai norādītu, vai ir atrastas atmiņas kļūdas. Piemērs:

Šeit ir darbību centra ikona: ![Darbību centra ikona](media/action-center-icon.png) 

Un paziņojuma paraugs: ![Nav atmiņas kļūdu](media/no-memory-errors.png)

Ja esat izlaidis paziņojumu, uzdevumjoslā varat atlasīt **darbību centra** ikonu, lai parādītu **darbību centru** un skatītu ritināmo paziņojumu sarakstu.

Lai pārskatītu detalizētu informāciju, uzdevumjoslas meklēšanas lodziņā ierakstiet **notikums** un pēc tam atlasiet **notikumu skatītājs**. **Notikumu skatītāja**kreisajā rūtī naviģējiet uz **Windows žurnālu > sistēmu**. Labajā rūtī skenējiet sarakstu, aplūkojot **avota** kolonnu, līdz brīdim, kad tiek parādīts notikumi ar avota vērtību **memorydiagnostics-rezultāti**. Izcelt katru šādu notikumu un redzēt rezultātu informāciju ailē zem cilnes **Vispārīgi** zem saraksta.
