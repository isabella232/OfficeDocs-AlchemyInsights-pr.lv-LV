---
title: MIM sinhronizācijas pakalpojuma konfigurēšana
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481871"
---
# <a name="configure-mim-sync-service"></a>MIM sinhronizācijas pakalpojuma konfigurēšana

Microsoft Identity Manager (MIM) sinhronizācijas pakalpojums ir MIM komponents. Tas ir centralizēts lokāls pakalpojums, kas saglabā un integrē informāciju organizācijām ar vairākiem lokāliem direktorijiem un datu bāzēm. Jūs, iespējams, varēsit novērst savu problēmu saistībā ar MIM sinhronizāciju, ja problēma ir novērsta jaunākajā atjauninājumā uz MIM vai ir viena no citām problēmām, kas minētas tālāk esošajā sadaļā.

**Ieteicamās darbības**

1. Pārliecinieties, vai izmantojat jaunāko MIM sinhronizācijas atjauninājumu, un atzīmējiet [MIM sinhronizācijas laidiena piezīmes](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) , lai noteiktu, vai problēma ir novērsta atjauninājumā.
2. Ja problēma ir saistīta ar vispārējo LDAP, vispārīgo SQL, Lotus Domino vai tīmekļa pakalpojumu savienotāju, pārliecinieties, vai izmantojat [vispārīgu savienotāju](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history)neseno atjauninājumu.
3. Ja MIM sinhronizācijas pieturas ar kļūdu, iepazīstieties ar [darbību kļūdu kodu](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) tabulu, lai noteiktu iespējamos iemeslus.
4. Ja opcija palaist apstājas ar **paplašinājumu-DLL — ir izņēmums**, pēc tam noklikšķiniet uz šiem vārdiem, lai atvērtu **savienotāja telpas objekta rekvizītu** logu, un noklikšķiniet uz **steka izsekošana...** , lai skatītu plašāku informāciju par galveno iemeslu, kā aprakstīts sadaļā [paplašinājums-DLL — Izņēmums](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).
5. Ja paziņojuma par paroļu mainīšanas pakalpojuma (RKN) komponentu ziņojumos **radās kļūda 6025** paroļu sinhronizēšanas laikā, skatiet rokasgrāmatu par problēmu novēršanas informāciju par [rkn ziņošanas kļūdu 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).
6. Ja pilna sinhronizācija ar FIM pakalpojumu pārvaldības aģentu darbojas lēni, atzīmējiet izvēles rūtiņu **automātiski palielināt** TempDB, kā tas ir aprakstīts rakstā [lēna vai pilna sinhronizācijas problēmu novēršana](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).
7. Ja, izmantojot FIM Service Management Agent, tiek rādīts kļūdas ziņojums par apturēšanas serveri ar neveiksmīgiem tīmekļa pakalpojumiem, skatiet sadaļu [atbalsts-informācija: neizveidotie tīmekļa pakalpojumi](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) , lai iegūtu pārskatu par cēloni.

