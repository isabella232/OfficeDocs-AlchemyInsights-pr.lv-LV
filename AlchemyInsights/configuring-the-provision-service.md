---
title: Nodrošināšana pakalpojuma konfigurēšana
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: 271ab7ad34c0f85f6f5a9d8d3dc2d901fe6fe8f978a2cc98eed986f594036f17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54033285"
---
# <a name="configuring-the-provision-service"></a>Nodrošināšana pakalpojuma konfigurēšana

Lai automatizēti lietotāju nodrošināšana darbotos, Azure AD pieprasa derīgus akreditācijas datus, kas ļauj izveidot savienojumu ar Workday tīmekļa pakalpojumu API. Papildus tiek validta arī poga Pārbaudīt savienojumu lietojumprogrammā Workday ad user Provisioning, arī pārbauda, vai var izveidot savienojumu ar Azure AD Savienošana nodrošināšanas aģentu, kas saistīts ar AD domēnu.

Ja Azure portāls atgriež kļūdu, saglabājot akreditācijas datus, veiciet tālāk norādītās ieteicamās darbības:

1. Apstipriniet, ka esat konfigurējis Workday integrācijas sistēmas lietotāja kontu, kā norādīts apmācību sadaļā [Integrācijas sistēmas lietotāja konfigurēšana lietojumprogrammā Workday.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
2. Pārliecinieties, vai Azure AD Savienošana nodrošināšanas aģenta pakalpojums ir iestatīts un darbojas jūsu lokālajā Windows, izmantojot pakalpojumu pārvaldības konsoli. Varat arī pārbaudīt aģenta statusu Azure portālā, noklikšķinot uz pogas Skatīt lokālos aģentus.
3. Pārbaudiet, vai laukā "Workday Username" tiek ievadīta vērtība username@workday-nomnieka-nosaukums. Ja trūkst workday nomnieka nosaukuma, workday autentifikācija neizdodas.
4. Ja konfigurējot integrāciju ar Workday ieviešanas nomnieku, ņemiet vērā jūsu Workday nomnieka ieplānotās dīkstāves stundas. Darba diena ir ieplānojusi savu ieviešanas nomnieku laiku nedēļas nogalēs (parasti no vakarā līdz sestdienas rītam) un savienojamības kļūmes šajā dīkstāves logā ir zināma problēma, kas automātiski tiek novērsta, tiklīdz ieviešanas nomnieki atkal ir tiešsaistē.
5. Retos gadījumos šī kļūda var tikt parādīts arī tad, ja nomnieka atsvaidzināšanas dēļ ir mainīta integrācijas sistēmas lietotāja parole vai konts ir bloķēts vai ir beidzies derīgums. Lūdzu, pārbaudiet integrācijas sistēmas lietotāja statusu pie sava Darba dienas administratora.

Papildinformāciju par automātiskās nodrošināšanas darba dienas konfigurēšanu skatiet rakstā Apmācība: darba [dienas konfigurēšana automātiskai lietotāju nodrošināšana.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
