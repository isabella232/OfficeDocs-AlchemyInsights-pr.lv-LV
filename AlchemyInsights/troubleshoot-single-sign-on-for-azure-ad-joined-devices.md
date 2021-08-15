---
title: Vienotās pierakstīšanās problēmu novēršana Azure AD ierīcēs
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
- "9003246"
- "9327"
ms.openlocfilehash: 872333e13bb51b3a22431154627ad561f6db88c681c9eeee523fdd09e58c0371
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039253"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Vienotās pierakstīšanās problēmu novēršana Azure AD ierīcēs

Ja jums ir lokāla Active Directory (AD) vide un vēlaties savienot savus AD domēnu datorus ar Azure AD, varat to paveikt, veicot hibrīdu Azure AD savienojumu. [Kā: Plānojiet hibrīdo Azure Active Directory pievienošanās ieviešanai](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) nodrošina saistītās darbības, lai ieviestu hibrīdu Azure AD savienojumu jūsu vidē.

Papildinformāciju skatiet rakstā Azure AD pievienoto ierīču konfigurēšana lokālajām Single-Sign [ierīcēs, izmantojot Windows Hello darbam](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).

**Primārās atsvaidzināšanas pilnvaras (PRIMARY Refresh Token – PRT) problēmas**

Primārā atsvaidzināšanas pilnvara (Primary Refresh Token – PRT) ir Azure AD autentifikācijas galvenā artefaktu ierīcēs Windows 10, Windows Server 2016 un jaunākās versijās, iOS un Android ierīcēs. Tas ir JSON tīmekļa marķieris (JSON Web Token — JWT), kas ir īpaši izsniegts Microsoft pirmās puses marķieru vekseļi, lai iespējotu vienoto pierakstīšanu (single sign-on — SSO) visās lietojumprogrammās, kas tiek izmantotas šajās ierīcēs. Detalizētu informāciju par PRT izdotu, lietošanu un aizsargāšanu Windows 10 ierīcēs skatiet rakstā Kas ir [primārās atsvaidzināšanas pilnvara?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: YES un AzureADPrt: YES**

Šie lauki norāda, vai lietotājs ir sekmīgi autentificējis Azure AD, pierakstoties ierīcē. Ja vērtības ir **NO**, tās var būt šādu iemeslu dēļ:

- Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)
- Alternatīvais pieteikšanās ID
- HTTP starpniekserveris nav atrasts

Lai novērstu problēmas ierīcēs, izmantojot komandu dsregcmd, skatiet [rakstu SSO stāvoklis.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
