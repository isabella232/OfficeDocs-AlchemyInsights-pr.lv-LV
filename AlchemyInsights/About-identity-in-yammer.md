---
title: Par identitāti pakalpojumā Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148310"
---
# <a name="about-identity-in-yammer"></a>Par identitāti pakalpojumā Yammer

Ieteicams visiem tīkliem veikt šādas darbības, lai izvairītos no problēmām, kas saistītas ar identitāti:

1. Ieviest Office 365 identitāti pēc microsoft 365 kontu nodrošināšanas lietotājiem Azure AD, lai nodrošinātu, ka visi lietotāji pierakstās, izmantojot savu primāro Microsoft 365 kontu. Papildinformāciju skatiet rakstā [Office 365 identitātes ieviešana Yammer lietotājiem](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. Konsolidēt vairākus Yammer tīklus. Legacy Yammer konfigurācijas ļauj vairākiem Yammer tīkliem izveidot savienojumu ar vienu nomnieku. Papildinformāciju skatiet sadaļā Tīkla [migrācija — vairāku Yammer tīklu konsolidēšana](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. Pēc izvēles ieviest yammer licencēšanu, lai bloķētu lietotājus no Yammer, ja viņiem nav licences. Papildinformāciju skatiet rakstā [Yammer lietotāju licenču pārvaldība pakalpojumā Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Visbeidzot, auditējiet lietotāju sarakstu vecākiem Yammer tīkliem un aizturēt mantotos lietotājus. Ieteicams aizturēt (deaktivizēt) lietotājus, nevis dzēst tos, jo dzēšana ir neatgriezeniska. Papildinformāciju skatiet rakstā Yammer [lietotāju audits tīklos, kas savienoti ar Office 365, un](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) [Lietotāju noņemšana](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

Konfigurējot Yammer, veicot šīs darbības, varat arī konfigurēt Yammer tīklu microsoft 365 vietējais režīms. Papildinformāciju skatiet rakstā [Yammer tīkla konfigurēšana microsoft 365 vietējais režīms](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).