---
title: Windows atmiņas diagnostikas palaišana operētājsistēmā Windows 10
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
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826674"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Windows atmiņas diagnostikas palaišana operētājsistēmā Windows 10

Ja jūsu datorā operētājsistēma Windows un programmas avarē, sasalst vai darbojas nestabilā veidā, iespējams, radusies problēma ar datora atmiņu (RAM). Varat palaist Windows atmiņas diagnostiku, lai meklētu problēmas saistībā ar datora RAM.

Uzdevumjoslas meklēšanas lodziņā ierakstiet atmiņas **diagnostika un** pēc tam atlasiet **Windows atmiņas diagnostika**. 

Lai palaistu diagnostiku, dators ir jārestartē. Varat restartēt tūlīt (lūdzu, vispirms saglabāt savu darbu un aizvērt atvērtos dokumentus un e-pasta ziņojumus) vai ieplānot diagnostikas automātisku pašanu nākamajā datora restartēšanas reizē:

![Windows atmiņas diagnostika](media/windows-memory-diagnostic.png)

Pēc datora restartēšanas automātiski tiek **palaists Windows atmiņas diagnostikas** rīks. Statuss un norise tiks parādītas, palaižot diagnostiku, un jums ir iespēja  atcelt diagnostiku, nospiežot tastatūras taustiņu ESC.

Kad diagnostika ir pabeigta, Windows tiks startēta kā parasti.
Uzreiz pēc restartēšanas, kad tiek parādīta darbvirsma,  uzdevumjoslā tiek parādīts paziņojums (blakus darbību centra ikonai), lai norādītu, vai ir atrastas atmiņas kļūdas. Piemēram:

Tālāk ir redzama darbību centra ikona. ![Darbību centra ikona](media/action-center-icon.png) 

Un paziņojuma paraugs: ![Atmiņas kļūdu nav](media/no-memory-errors.png)

Ja nepamanīāt paziņojumu,  varat atlasīt darbību centra ikonu  uzdevumjoslā, lai atvērtu darbību centru un skatītu ritināmu paziņojumu sarakstu.

Lai pārskatītu detalizētu informāciju, **ierakstiet notikums** uzdevumjoslas meklēšanas lodziņā un pēc tam atlasiet **Notikumu skatītājs**. Notikumu **skatītāja** kreisajā rūtī naviģējiet uz **Windows žurnālus > sistēmu**. Labajā rūtī noskenējiet sarakstu, vienlaikus aplūkojot kolonnu Avots, līdz tiek atvērts notikums ar avota vērtību **MemoryDiagnostics-Results.**  Iezīmējiet katru šādu notikumu un skatiet rezultātu informāciju lodziņā zem **cilnes** Vispārīgi zem saraksta.
