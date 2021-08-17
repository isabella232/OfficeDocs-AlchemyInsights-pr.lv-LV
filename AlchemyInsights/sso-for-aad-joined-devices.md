---
title: Single-Sign ierīcēs, Azure Active Directory ierīcēs, kurās ir savienojums
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: 365225926296677feb7853481651a634792fd8bfa9abd9dc9359ffaae50b60eb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050017"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Vienotā pierakstīšanās Azure Active Directory ierīcēs, kas ir Azure Active Directory

Ja jums ir lokāla Active Directory (AD) vide un vēlaties savienot savus AD domēnu datorus ar Azure AD, varat to paveikt, veicot hibrīdu Azure AD savienojumu. [Kā: Plānojiet hibrīdo Azure Active Directory pievienošanās ieviešanai](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) nodrošina saistītās darbības, lai ieviestu hibrīdu Azure AD savienojumu jūsu vidē.

[Azure AD pievienoto ierīču konfigurēšana lokālajās ierīcēs Single-Sign izmantojot Windows Hello darbam](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Primārās atsvaidzināšanas pilnvaras (PRIMARY Refresh Token – PRT) problēmas** Primārā atsvaidzināšanas pilnvara (Primary Refresh Token – PRT) ir Azure AD autentifikācijas galvenā artefaktu ierīcēs Windows 10, Windows Server 2016 un jaunākās versijās, iOS un Android ierīcēs. Tas ir JSON tīmekļa marķieris (JSON Web Token — JWT), kas ir īpaši izsniegts Microsoft pirmās puses marķieru vekseļi, lai iespējotu vienoto pierakstīšanu (single sign-on — SSO) visās lietojumprogrammās, kas tiek izmantotas šajās ierīcēs. [Sadaļā Kas ir primārās atsvaidzināšanas pilnvara?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)mēs sniedzsim detalizētu informāciju par PRT izrakstīšanu, lietošanu un aizsardzību Windows 10 ierīcēs.

**WamDefaultSet: YES un AzureADPrt: YES** Šie lauki norāda, vai lietotājs ir sekmīgi autentificējis Azure AD, pierakstoties ierīcē. Ja vērtības ir **NO**, tam varētu būt iemesls:

- Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).
- Alternatīvais pieteikšanās ID
- HTTP starpniekserveris nav atrasts

Problēmu novēršana ierīcēs, izmantojot komandu dsregcmd — [SSO stāvoklis](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
