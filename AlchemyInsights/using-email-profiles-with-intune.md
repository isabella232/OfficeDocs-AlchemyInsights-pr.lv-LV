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
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653295"
---
# <a name="using-email-profiles-with-intune"></a>E-pasta profilu izmantošana ar Intune

Intune var izmantot, lai izveidotu un izvietotu e-pasta profilus vietējā (iebūvētā) e-pasta klientam vairāku ierīču platformās.

Lai iegūtu informāciju par dažiem ierobežojumiem, kas saistīti ar e-pasta profiliem, tostarp to, kā tiek apstrādāti esošie profili un kā noņemt e-pasta profilus, skatiet rakstu [e-pasta iestatījumu pievienošana ierīcēs, izmantojot Intune](https://docs.microsoft.com/intune/email-settings-configure).

Lai iegūtu papildinformāciju par to, kā izveidot e-pasta profilus katrai ierīču platformai, skatiet:

[Android ierīces iestatījumi, lai pakalpojumā Intune konfigurētu e-pastu, autentifikāciju un sinhronizāciju](https://docs.microsoft.com/intune/email-settings-android)  
[E-pasta iestatījumu pievienošana operētājsistēmā iOS un iPadOS ierīcēs programmā Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[E-pasta profila iestatījumi pakalpojumā Microsoft Intune ierīcēs, kurās darbojas operētājsistēma Windows Phone 8,1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[E-pasta profila iestatījumi ierīcēm, kurās darbojas Windows 10 programmā Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Kopējā sinhronizācijas problēma**

**KNOX Android e-pasta profils neļauj sinhronizēt lietotāju kontaktpersonas, kalendārus un uzdevumus.**

KNOX tehnoloģiju KNOX e-pasta profils piedāvā administratoram iespēju izlemt, kuri satura tipi ir sinhronizēti ar ierīci, iestatot katru iespējoto.

Ja iestatījums jebkuram satura tipam ir iestatīts uz **nav konfigurēts** (noklusējums), šis satura tips netiek sinhronizēts automātiski. Lietotājs var iespējot satura tipu, ko tie vēlas veikt tieši ierīcē manuāli, taču šī konfigurācija tiek pārrakstīta, izmantojot Intune politikas iestatījumu, un šī satura tipa sinhronizācijas pieturas.

