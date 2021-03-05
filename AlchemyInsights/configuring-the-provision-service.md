---
title: Pakalpojumu sniedzēja konfigurēšana
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
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482871"
---
# <a name="configuring-the-provision-service"></a>Pakalpojumu sniedzēja konfigurēšana

Lai veiktu automātisku lietotāja nodrošināšanu darbam, Azure AD ir nepieciešami derīgie akreditācijas dati, kas ļauj izveidot savienojumu ar darbadienu tīmekļa pakalpojumu API. Tālāk poga testa savienojums, kas pieejama sadaļā WORKDAY to AD User nodrošināšanas programma, validē arī, ja tā var izveidot savienojumu ar Azure AD Connect nodrošināšanas aģentu, kas saistīts ar reklāmas domēnu.

Ja Azure portāls atgriež kļūdu, saglabājot akreditācijas datus, rīkojieties šādi:

1. Apstipriniet, ka esat konfigurējis darba dienu integrācijas sistēmas lietotāja kontu, kā norādīts sadaļā apmācība [konfigurējiet integrācijas sistēmas lietotāju darbdienas](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)ietvaros.
2. Pārliecinieties, vai Azure AD Connect nodrošināšanas aģenta pakalpojums darbojas jūsu lokālajā Windows serverī, izmantojot pakalpojumu pārvaldības konsoli. Varat arī pārbaudīt aģenta statusu Azure portālā, noklikšķinot uz pogas Skatīt lokālos aģentus.
3. Pārliecinieties, vai ievadāt lauka "WORKDAY username" vērtību, izmantojot formātu username@workday nomnieka vārdu. Ja nav ievadīts darbdienas nomnieka vārds, darba dienu autentifikācija neizdevās.
4. Ja konfigurējat integrāciju ar WORKDAY implementēšanas nomnieku, ņemiet vērā sava darba dienu nomnieka plānotās dīkstāves stundas. Funkcija WORKDAY ir ieplānojusi noteiktu laiku tās implementēšanai uz nedēļas nogales (parasti no piektdienas vakara līdz sestdienas rītam) un savienojamības kļūmes šajā dīkstāves logā ir zināma problēma, kas automātiski tiek novērsta, tiklīdz ieviešanas nomnieki atkal ir tiešsaistē.
5. Retos gadījumos, iespējams, redzēsit šo kļūdu, ja ir mainīta integrācijas sistēmas lietotāja parole, jo nomnieka atsvaidzināšana vai konts ir bloķēts vai beidzies derīguma termiņš. Lūdzu, pārbaudiet integrācijas sistēmas lietotāja statusu ar savu darba dienu administratoru.

Lai iegūtu papildinformāciju par to, kā konfigurēt darba dienu automatizētai konfigurēšanai, skatiet rakstu [apmācība: darbdienas konfigurēšana automātiskai lietotāju nodrošināšanai](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).
