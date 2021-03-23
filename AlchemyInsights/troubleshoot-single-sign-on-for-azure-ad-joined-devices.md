---
title: Vienas pierakstīšanās pakalpojumam Azure AD savienotajām ierīcēm problēmu novēršana
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
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036173"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Vienas pierakstīšanās pakalpojumam Azure AD savienotajām ierīcēm problēmu novēršana

Ja jums ir lokālā Active Directory (AD) vide un vēlaties pievienoties savam AD Domain-Joined datoriem Azure AD, varat to paveikt, veicot hibrīda Azure AD savienojumu. [Kā: plānojiet Hibrīdā Azure Active Directory pievienošanas implementācijā](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) ir aprakstītas darbības, kas jāveic, lai nodrošinātu Hibrīdā Azure AD savienojumu savā vidē.

Papildinformāciju skatiet rakstā [AZURE ad savienoto ierīču konfigurēšana lokālajā Single-Sign, izmantojot Windows Hello darbam](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).

**Primārās atsvaidzināšanas marķierierīces (PRT) problēmas**

Primārā atsvaidzināšanas pilnvara (PRT) ir Azure AD autentifikācijas galvenais artefakts operētājsistēmā Windows 10, Windows Server 2016 un jaunākās versijās, iOS un Android ierīcēs. Tā ir JSON tīmekļa pilnvara (JWT), kas īpaši izsniegta Microsoft pirmās puses žetonu brokeriem, lai iespējotu vienotās pierakstīšanās (SSO) visās šajās ierīcēs lietotajās lietojumprogrammās. Detalizētu informāciju par to, kā PRT tiek izsniegta, lietota un aizsargāta Windows 10 ierīcēs, skatiet rakstā [kas ir primārā atsvaidzināšanas pilnvara?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: Jā un AzureADPrt: Jā**

Šie lauki norāda, vai lietotājs, pierakstoties ierīcē, ir sekmīgi autentificējis Azure AD. Ja **vērtības ir tādas, tās iemesls** var būt:

- Nederīga krātuves atslēga TPM, kas ir saistīts ar ierīci reģistrācijas laikā (pārbaudiet KeySignTest, kamēr darbojas paaugstināts)
- Alternatīvā pieteikšanās ID
- HTTP starpniekserveris nav atrasts

Lai novērstu ierīces, kas izmanto komandu dsregcmd, skatiet sadaļu [SSO statuss](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).
