---
title: Pierakstīšanās operētājsistēmā Windows 10, neizmantojot paroli
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830553"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Pierakstīšanās operētājsistēmā Windows 10, neizmantojot paroli

Lai izvairītos no nepieciešamības ievadīt paroli Windows startēšanas laikā, ieteicams izmantot kādu no Windows Hello drošās pierakstīšanās opcijām, piemēram, PIN, sejas atpazīšanu vai pirksta nospiedumu, ja tāda ir pieejama. Ja tiešām vēlaties atspējot drošo pierakstīšanu, skatiet tālāk esošos norādījumus "Automātiska pierakstīšanās sistēmā Windows 10".

**Kā aizsargāt Windows Hello alternatīvas konta parolei**

Dodieties **uz > konti > Pierakstīšanās opcijas** (vai noklikšķiniet [šeit).](ms-settings:signinoptions?activationSource=GetHelp) Tiks uzskaitītas pieejamās pierakstīšanās opcijas. Piemēram:

![Pierakstīšanās opcijas.](media/sign-in-options.png)

Noklikšķiniet uz vai pieskarieties pie vienas no opcijām, lai to konfigurētu. Nākamreiz, kad startēsit vai atbloķēsit sistēmu Windows, varēsit izmantot jauno opciju, nevis paroli. 

**Automātiska pierakstīšanās operētājsistēmā Windows 10**

**Piezīme.** Automātiskā pierakstīšanās ir ērta, taču rada drošības risku, īpaši, ja jūsu dators ir pieejams vairākiem cilvēkiem. 

1. Uzdevumjoslā **noklikšķiniet uz** vai pieskarieties pie pogas Sākt.

2. Ierakstiet **netplwiz** un nospiediet taustiņu Enter, lai atvērtu logu Lietotāju konti.

3. Izvēlnē **Lietotāju konti** noklikšķiniet uz konta, kurā vēlaties automātiski pierakstīties sistēmas Windows startēšanas laikā.

4. Notīriet izvēles rūtiņu Lai izmantotu šo datoru, lietotājiem ir jāievada lietotājvārds un parole.

    ![Lietotājiem ir jāievada lietotājvārda un paroles opcija.](media/users-must-enter-username.png)

5. Noklikšķiniet uz **Labi**. Jums tiks lūgts ievadīt un apstiprināt atlasītā konta paroli. Noklikšķiniet **uz Labi,** lai pabeigtu. Nākamajā Windows 10 startēšanas reizē tā automātiski pierakstīsies atlasītajā kontā.
