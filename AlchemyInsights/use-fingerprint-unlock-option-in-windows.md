---
title: Pirksta nospiedumu atbloķēšanas opcijas izmantošana operētājsistēmā Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796684"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Pirksta nospiedumu atbloķēšanas opcijas izmantošana operētājsistēmā Windows 10

**Iespējot Windows Hello pirkstu nospiedumu**

Lai atbloķētu windows 10, izmantojot pirksta nospiedumu, ir jāiestata Windows Hello pirksta nospiedums, pievienojot (ļaujot Windows uzzināt, kā to atpazīt) vismaz vienu pirkstu. 

1. Dodieties **uz > konti > Pierakstīšanās opcijas** (vai noklikšķiniet [šeit).](ms-settings:signinoptions?activationSource=GetHelp) Tiks uzskaitītas pieejamās pierakstīšanās opcijas. Piemēram:

    ![Pierakstīšanās opcijas.](media/sign-in-options.png)

2. Noklikšķiniet uz vai pieskarieties pie **Windows Hello pirksta nospiedumu** un pēc tam **noklikšķiniet uz Iestatīt**. Windows Hello iestatīšanas logā noklikšķiniet uz **Sākt darbu.** Tiks aktivizēts pirkstu nospiedumu sensors, un jums tiks lūgts novietot pirkstu uz sensora:

   ![Pirkstu nospiedumu sensors.](media/fingerprint-sensor.png)

3. Izpildiet norādījumus, kas lūgs atkārtoti skenēt pirkstu. Kad tas ir izdarīts, varat pievienot citus pirkstus, kurus, iespējams, vēlēsities izmantot, lai pierakstītos. Nākamreiz, kad pierakstīsties operētājsistēmā Windows 10, jums būs iespēja izmantot pirksta nospiedumu, lai to izdarītu.

**Windows Hello pirkstu nospiedumu nav pieejama kā pierakstīšanās opcija**

Ja opcija Pierakstīšanās opcijas netiek rādīta, izmantojot Windows Hello pirkstu nospiedumu, sistēma Windows neizmanto jūsu datoram pievienoto pirkstu nospiedumu lasītāju/skeneri vai arī sistēmas politika neļauj to izmantot (ja, piemēram, jūsu datoru pārvalda jūsu darbvieta).  Lai novērstu problēmas, 

1. **Uzdevumjoslā** atlasiet pogu Sākums un meklējiet **Ierīču pārvaldnieks**.

2. Noklikšķiniet uz vai pieskarieties, lai **atvērtu ierīču pārvaldnieku**.

3. Ierīču pārvaldniekā izvērsiet biometriskās ierīces, noklikšķinot uz tās skujiņas.

   ![Biometriskas ierīces.](media/biometric-devices.png)

4. Jūsu pirkstu nospiedumu skenerim ir jābūt norādītam kā biometriskai ierīcei, piemēram, sinaptikas WBDI skenerim:

   ![Biometriskas ierīces.](media/biometric-devices-expanded.png)

5. Ja jūsu pirkstu nospiedumu skeneris nav redzams un skeneris ir integrēts jūsu datorā, dodieties uz datora ražotāja tīmekļa vietni. Datora modeļa tehniskā atbalsta sadaļā meklējiet Windows 10 draiveri, ko instalēt.

6. Ja skeneris nav dators (pievienots, izmantojot USB), dodieties uz skenera ražotāja tīmekļa vietni, lai atrastu un instalētu Windows 10 ierīces draivera programmatūru jūsu skenera modelim.
