---
title: Pirkstu nospiedumu atbloķēšanas opcijas lietošana operētājsistēmā Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795251"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Pirkstu nospiedumu atbloķēšanas opcijas lietošana operētājsistēmā Windows 10

**Windows Hello Fingerprint iespējošana**

Lai atbloķētu Windows 10, izmantojot pirkstu nospiedumu, ir jāiestata Windows Hello Fingerprint, pievienojot (ļaujot Windows uzzināt atpazīst) vismaz vienu pirkstu. 

1. Dodieties uz **sadaļu iestatījumi > konti > pierakstīšanās opcijas** (vai noklikšķiniet [šeit](ms-settings:signinoptions?activationSource=GetHelp)). Būs norādītas pieejamās pierakstīšanās opcijas. Piemērs:

    ![Pierakstīšanās opcijas.](media/sign-in-options.png)

2. Noklikšķiniet uz vai pieskarieties pie **Windows Hello Fingerprint**, pēc tam noklikšķiniet uz **Iestatīt**. Windows Hello uzstādīšanas logā noklikšķiniet uz **Sākt darbu**. Pirkstu nospiedumu sensors tiks aktivizēts, un jums tiks lūgts novietot pirkstu uz sensora:

   ![Pirkstu nospiedumu sensors.](media/fingerprint-sensor.png)

3. Izpildiet norādījumus, kas lūgs atkārtoti skenēt pirkstu. Kad tas ir izdarīts, jums būs iespēja pievienot citus pirkstus, kurus varat izmantot, lai pierakstītos. Nākamreiz, kad pierakstīsities operētājsistēmā Windows 10, jums būs iespēja izmantot savu pirksta nospiedumu.

**Windows Hello Fingerprint nav pieejama kā pierakstīšanās opcija**

Ja Windows Hello pirksta nospiedums netiek rādīts kā opcija **pierakstīšanās opcijās**, tas nozīmē, ka Windows nezina nevienu pirkstu nospiedumu lasītāju/skeneri, kas pievienots datoram, vai sistēmas politika neļauj to izmantot (ja, piemēram, jūsu datoru pārvalda jūsu darbvieta). Lai novērstu problēmu: 

1. Uzdevumjoslā atlasiet pogu **Sākums** un meklējiet **ierīču pārvaldnieks**.

2. Noklikšķiniet vai pieskarieties, lai atvērtu **ierīču pārvaldnieku**.

3. Ierīču pārvaldniekā izvērsiet biometrijas ierīces, noklikšķinot uz tās v veida.

   ![Biometrijas ierīces.](media/biometric-devices.png)

4. Jūsu pirkstu nospiedumu skenerim ir jābūt norādītam kā biometriskai ierīcei, piemēram, Synaptics WBDI skenerim:

   ![Biometrijas ierīces.](media/biometric-devices-expanded.png)

5. Ja netiek parādīts jūsu pirkstu nospiedumu skeneris un skeneris ir iebūvēts datorā, atveriet datora ražotāja tīmekļa vietni. Datora modeļa sadaļā tehniskais atbalsts meklējiet Windows 10 draiveri rīkam, ko varat instalēt.

6. Ja skeneris ir atdalīts no datora (pievienots, izmantojot USB), dodieties uz skenera ražotāja tīmekļa vietni, lai atrastu un instalētu Windows 10 ierīču draiveru programmatūru jūsu skenera modelim.
