---
title: Par identitāti programmā Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 57e7e6328747fc05b89799d631b2c6d7e0056547253aa3d75cdecb38cea3ad7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918944"
---
# <a name="about-identity-in-yammer"></a>Par identitāti programmā Yammer

Ir ieteicams visos tīklos veikt tālāk norādītās darbības, lai izvairītos no ar identitāti saistītām problēmām.

1. Ieviest Office 365 identitāti pēc Microsoft 365 nodrošināšanas lietotājiem pakalpojumā Azure AD, lai nodrošinātu, ka visi lietotāji pierakstās, izmantojot savu primāro Microsoft 365 kontu. Papildinformāciju skatiet [rakstā Office 365 identitātes Yammer lietotājiem.](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity)
2. Vairāku tīkla Yammer konsolidēšanu. Mantotas Yammer konfigurācijas ļauj izveidot Yammer tīklu savienojumu ar vienu nomnieku. Papildinformāciju skatiet rakstā [Tīkla migrācija — vairāku Yammer tīklu konsolidēšana.](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)
3. Ja vēlaties, ieviesiet Yammer, lai lietotājiem bloķētu Yammer, ja viņiem nav licences. Papildinformāciju skatiet [rakstā Yammer licenču pārvaldība Office 365.](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)
4. Visbeidzot auditēt lietotāju sarakstu vecākiem Yammer tīkliem un apturēt mantoto lietotāju darbību. Ir ieteicams aizturēt (deaktivizēt) lietotājus, nevis tos izdzēst, jo dzēšana ir neatgriezeniska. Papildinformāciju skatiet rakstā [Auditēšana Yammer tīklos, kas savienoti ar Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) [un Noņemt lietotājus.](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users)

Konfigurējot Yammer veicot šīs darbības, varēsit arī konfigurēt savu Yammer tīklu vietējā režīmā Microsoft 365. Papildinformāciju skatiet rakstā [Sava Yammer tīkla konfigurēšana vietējā režīmā Microsoft 365.](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode)