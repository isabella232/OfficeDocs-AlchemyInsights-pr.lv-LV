---
title: Izmantojiet pirkstu nospiedumu atbloķēšanas opciju operētājsistēmā Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 8a5059c722c306ad79811140062cec7f52f31766
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588322"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Izmantojiet pirkstu nospiedumu atbloķēšanas opciju operētājsistēmā Windows 10

**Iespējot Windows Hello pirksta nospiedumu**

Lai atbloķētu operētājsistēmu Windows 10, izmantojot pirksta nospiedumu, ir jāiestata Windows Hello pirksta nospiedums, pievienojot (ļaujot Windows iemācīties atpazīt) vismaz vienu pirkstu. 

1. Dodieties uz **iestatījumi > konti > pierakstīšanās opcijas** (vai noklikšķiniet [šeit](ms-settings:signinoptions?activationSource=GetHelp)). Tiks uzskaitītas pieejamās pierakstīšanās opcijas. Piemērs:

    ![Pierakstīšanās opcijas.](media/sign-in-options.png)

2. Noklikšķiniet uz vai pieskarieties **Windows Hello pirksta nospiedums**, pēc tam noklikšķiniet uz **Iestatīt**. Windows Hello iestatīšanas logā noklikšķiniet uz **Sākt darbu**. Pirkstu nospiedumu sensors aktivizēs, un jums tiks lūgts novietot pirkstu uz sensora:

   ![Pirkstu nospiedumu sensors.](media/fingerprint-sensor.png)

3. Izpildiet norādījumus, kas prasīs atkārtoti skenēt pirkstu. Kad tas ir izdarīts, jums būs iespēja pievienot citus pirkstus, kurus jūs varētu vēlēties izmantot pierakstīšanās gadījumā. Nākamreiz, kad pierakstīsies operētājsistēmā Windows 10, jums būs iespēja izmantot pirksta nospiedumu.

**Windows Hello pirksta nospiedums nav pieejams kā pierakstīšanās opcija**

Ja Windows Hello pirksta nospiedums nav redzams kā opcija **pierakstīšanās opcijas**, tas nozīmē, ka Windows nav informēts par jebkuru pirkstu nospiedumu lasītāju/skeneri, kas ir pievienots datoram, vai arī sistēmas politika liedz tās izmantošanu (piemēram, ja jūsu datoru pārvalda darbvieta). Lai novērstu: 

1. Uzdevumjoslā atlasiet pogu **Sākums** un meklējiet **ierīču pārvaldnieks**.

2. Noklikšķiniet uz vai pieskarieties, lai atvērtu **ierīču pārvaldnieku**.

3. Ierīču pārvaldniekā izvērsiet sadaļu biometrijas ierīces, noklikšķinot uz tās Chevron.

   ![Biometrijas ierīcēm.](media/biometric-devices.png)

4. Jūsu pirkstu nospiedumu skeneris ir jānorāda kā biometriskā ierīce, piemēram, Synaptics WBDI Scanner:

   ![Biometrijas ierīcēm.](media/biometric-devices-expanded.png)

5. Ja pirkstu nospiedumu skeneris netiek rādīts un skeneris ir integrēts datorā, apmeklējiet datora ražotāja vietni. DATORA modeļa sadaļā tehniskā palīdzība meklējiet skenera Windows 10 draiveri, ko varat instalēt.

6. Ja skeneris ir atdalīts no datora (pievienots, izmantojot USB), apmeklējiet skenera ražotāja vietni, lai atrastu un instalētu Windows 10 ierīces draivera programmatūru savam skenera modelim.
