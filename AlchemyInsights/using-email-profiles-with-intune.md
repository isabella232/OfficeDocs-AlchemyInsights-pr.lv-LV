---
title: E-pasta profilu izmantošana ar Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: b1653b73e7296e7eed411ae73c19342a1187b2eb7e287cff4339ea0ca32d75c1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919430"
---
# <a name="using-email-profiles-with-intune"></a>E-pasta profilu izmantošana ar Intune

Intune var izmantot, lai izveidotu un izvietotu e-pasta profilus iebūvētajam (iebūvētajam) e-pasta klientam vairākās ierīču platformās.

Informāciju par dažiem ierobežojumiem, kas saistīti ar e-pasta profiliem, tostarp to, kā tiek apstrādāti esošie profili un kā noņemt e-pasta profilus, skatiet rakstā E-pasta iestatījumu pievienošana ierīcēm, izmantojot [Intune](https://docs.microsoft.com/intune/email-settings-configure).

Papildinformāciju par to, kā izveidot e-pasta profilus katrai ierīces platformai, skatiet tālāk redzamajā rakstā.

[Android ierīces iestatījumi e-pasta, autentifikācijas un sinhronizācijas konfigurēšanai Intune](https://docs.microsoft.com/intune/email-settings-android)  
[E-pasta iestatījumu pievienošana iOS un iPadOS ierīcēm programmā Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[E-pasta profila iestatījumi programmā Microsoft Intune ierīcēm, kurās darbojas Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[E-pasta profila iestatījumi ierīcēm, kurās Windows 10 instalēta Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Bieži sastopama sinhronizācijas problēma**

**KNOX android e-pasta profilā lietotāja kontaktpersonas, kalendārs un uzdevumi netiek sinhronizēti ar lietotāju ierīcēm.**

KNOX android KNOX e-pasta profilā administratoram tiek piedāvāta opcija izlemt, kuri satura tipi tiek sinhronizēti ar ierīci, iestatot katra satura iespējošanu.

Ja kāda satura tipa iestatījums ir **Nav** konfigurēts (noklusējums), šis satura tips netiek sinhronizēts automātiski. Lietotājs var iespējot satura tipu, kuru tas vēlas tieši ierīcē manuāli, bet šo konfigurāciju pārraksta Intune politikas iestatījums, un šim satura tipam sinhronizācija tiek apturēta.

