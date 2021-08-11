---
title: Startēšanas iestatījumi programmā Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: 526b92013f26675b5bf42077271ae7dc7003af31fa8f605d76aea92e0ccabfa1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53909833"
---
# <a name="startup-settings-in-windows-10"></a>Startēšanas iestatījumi programmā Windows 10

**Lietojumprogrammu automātiskas palaišanas mainīšana startēšanas laikā**

1. Dodieties [uz Iestatījumi > programmas > startēšanu](ms-settings:startupapps?activationSource=GetHelp).

2. Pārliecinieties, vai visas lietojumprogrammas, kuras vēlaties palaist startēšanas laikā, ir **ieslēgtas.**

**Programmas pievienošana automātiskai palaišanai startēšanas laikā**

1. Noklikšķiniet uz vai **pieskarieties pie** Sākt un atrodiet programmu, ko vēlaties palaist startēšanas laikā.

2. Ar peles labo pogu noklikšķiniet uz programmas, noklikšķiniet uz **Vēl un pēc** tam noklikšķiniet uz Atvērt faila **atrašanās vietu.** Tādējādi tiek atvērta atrašanās vieta, kur ir saglabāta saīsne uz programmu. Ja opcija Atvērt faila atrašanās vietu nav pieejama, tas nozīmē, ka programmu nevar palaist startēšanas laikā.

3. Kad faila atrašanās vieta ir atvērta, **nospiediet taustiņu kombināciju Windows logotipa taustiņš + R**, ierakstiet **shell:startup**, pēc tam noklikšķiniet uz **Labi**. Tiek atvērta startēšanas mape.

4. Nokopējiet un ielīmējiet saīsni uz programmu no faila atrašanās vietas startēšanas mapē.

**Startēšanas papildu opcijas (Seifs režīms, UEFI iestatījumi un palaišana no citas ierīces)**

1. Saglabājiet darbu un aizveriet visus atvērtos dokumentus, jo, izpildot šīs darbības, tiks restartēts dators.

2. Dodieties [uz Iestatījumi > atjaunināšanas & drošības > atkopšana.](ms-settings:recovery?activationSource=GetHelp)

3. Sadaļā **Startēšana ar papildu** noklikšķiniet uz Restartēt **tūlīt.** 

4. Pēc datora restartēšanas uz ekrānu Opcijas izvēle:

    - Lai varētu veikt sāknēšanu no ierīces, piemēram, USB diska, **noklikšķiniet uz Lietot ierīci**.

    - Lai ievadītu UEFI iestatījumus (dažreiz tiek dēvēti par BIOS iestatīšanu), noklikšķiniet uz Problēmu novēršana > Papildu **> UEFI aparātprogrammatūras Iestatījumi**. 

    - Lai atvērtu Seifs režīmu vai mainītu startēšanas papildu iestatījumus, noklikšķiniet uz Novērst > problēmas saistībā **> startēšanas Iestatījumi** un pēc tam noklikšķiniet uz **Restartēt.** Iespējams, jums tiks lūgts ievadīt [BitLocker atkopšanas atslēgu.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key) Pēc datora restartēšanas vēlreiz noklikšķiniet uz startēšanas iestatījuma, kuru vēlaties izmantot.