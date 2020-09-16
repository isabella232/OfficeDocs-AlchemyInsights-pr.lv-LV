---
title: Pierakstīšanās operētājsistēmā Windows 10, neizmantojot paroli
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719960"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Pierakstīšanās operētājsistēmā Windows 10, neizmantojot paroli

Lai izvairītos no paroles ievadīšanas Windows startēšanas laikā, iesakām izmantot kādu no Windows Hello drošās pierakstīšanās opcijām, piemēram, PIN, sejiņas atpazīšanu vai pirksta nospiedumu, ja tas ir pieejams. Ja tiešām vēlaties atspējot drošu pierakstīšanos, skatiet tālāk sniegtos norādījumus "automātiska pierakstīšanās Windows 10".

**Drošas Windows Hello alternatīvas konta parolei**

Dodieties uz **sadaļu iestatījumi > konti > pierakstīšanās opcijas** (vai noklikšķiniet [šeit](ms-settings:signinoptions?activationSource=GetHelp)). Būs norādītas pieejamās pierakstīšanās opcijas. Piemērs:

![Pierakstīšanās opcijas.](media/sign-in-options.png)

Noklikšķiniet uz vai pieskarieties vienai no opcijām, lai to konfigurētu. Nākamreiz, kad startējat vai atbloķējat Windows, paroles vietā varēsit izmantot jauno opciju. 

**Automātiska pierakstīšanās operētājsistēmā Windows 10**

**Piezīme**: automātiska pierakstīšanās ir ērta, taču ir ieviesti drošības riski, it īpaši tad, ja jūsu dators ir pieejams vairākām personām. 

1. Noklikšķiniet uz vai pieskarieties pie pogas **Sākt** uzdevumjoslā.

2. Ierakstiet **netplwiz** un nospiediet taustiņu ENTER, lai atvērtu lietotāju kontu logu.

3. **Lietotāju kontos**noklikšķiniet uz konta, kuram vēlaties automātiski pierakstīties, startējot sistēmu Windows.

4. Atzīmējiet izvēles rūtiņu "lietotājiem ir jāievada lietotājvārds un parole, lai izmantotu šo datoru".

    ![Lietotājiem ir jāievada lietotājvārds un parole.](media/users-must-enter-username.png)

5. Noklikšķiniet uz **Labi**. Jums būs jāievada un jāapstiprina atlasītā konta parole. Noklikšķiniet uz **Labi** , lai pabeigtu. Nākamreiz, kad tiks palaista operētājsistēma Windows 10, tā automātiski pierakstīsies atlasītajā kontā.
