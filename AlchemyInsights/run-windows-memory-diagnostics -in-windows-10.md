---
title: Atmiņas Windows palaišana programmā Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 63ba3afdd8f74b17559484f37e9250587aec9b4a929325d8f82e3c9ad06f1783
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53922578"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Atmiņas Windows palaišana programmā Windows 10

Ja Windows un programmas jūsu datorā avarē, sasalst vai darbojas nestabilā veidā, iespējams, radusies problēma ar datora atmiņu (RAM). Atmiņas diagnostiku var Windows, lai meklētu problēmas saistībā ar datora RAM.

Uzdevumjoslas meklēšanas lodziņā ierakstiet atmiņas **diagnostika un pēc** tam atlasiet Windows **Atmiņas diagnostika**. 

Lai palaistu diagnostiku, dators ir jārestartē. Varat restartēt tūlīt (lūdzu, vispirms saglabāt savu darbu un aizvērt atvērtos dokumentus un e-pasta ziņojumus) vai ieplānot diagnostikas automātisku pašanu nākamajā datora restartēšanas reizē:

![Windows Atmiņas diagnostika](media/windows-memory-diagnostic.png)

Pēc datora restartēšanas rīks **Windows diagnostikas** rīku. Statuss un norise tiks parādītas, palaižot diagnostiku, un jums ir iespēja  atcelt diagnostiku, nospiežot tastatūras taustiņu ESC.

Kad diagnostika ir pabeigta, Windows sāktos kā parasti.
Uzreiz pēc restartēšanas, kad tiek parādīta darbvirsma,  uzdevumjoslā tiek parādīts paziņojums (blakus darbību centra ikonai), lai norādītu, vai ir atrastas atmiņas kļūdas. Piemēram:

Tālāk ir redzama darbību centra ikona. ![Darbību centra ikona](media/action-center-icon.png) 

Un paziņojuma paraugs: ![Atmiņas kļūdu nav](media/no-memory-errors.png)

Ja nepamanīāt paziņojumu,  varat atlasīt darbību centra ikonu  uzdevumjoslā, lai atvērtu darbību centru un skatītu ritināmu paziņojumu sarakstu.

Lai pārskatītu detalizētu informāciju, **ierakstiet notikums** uzdevumjoslas meklēšanas lodziņā un pēc tam atlasiet **Notikumu skatītājs**. Notikumu **skatītāja** kreisās puses rūtī naviģējiet uz Windows **žurnālu > sistēmu**. Labajā rūtī noskenējiet sarakstu, vienlaikus aplūkojot kolonnu Avots, līdz tiek atvērts notikums ar avota vērtību **MemoryDiagnostics-Results.**  Iezīmējiet katru šādu notikumu un skatiet rezultātu informāciju lodziņā zem **cilnes** Vispārīgi zem saraksta.
