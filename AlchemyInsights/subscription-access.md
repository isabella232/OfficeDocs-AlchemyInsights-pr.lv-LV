---
title: Piekļuve abonementam
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003799"
- "6805"
ms.openlocfilehash: b138c05e87e70c18bb6528819a34f8a9501446d57dcf4dbac0734f70fbc3466b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999247"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Nevar pierakstīties Azure pārlūkprogrammas problēmu dēļ (pārlūkprogramma uzkaras, griežas, netiek ielādēta utt.)

Iespējams, jūsu darbības pārtraukums jūs ietekmē. Lūdzu, pārbaudiet, vai pašlaik pastāv pārtraukums: [Azure darbspējas statuss](https://status.azure.com/status/history/).

Lūdzu, atsakieties no visām aktīvajām Azure sesijām. Sāciet privātu vai inkognito režīmu savā tīmekļa pārlūkprogrammā.

Varat arī mēģināt atsvaidzināt pārlūkprogrammu, izmantot citu pārlūkprogrammu un dzēst kešatmiņas sīkfailus, ja iepriekš minētie nedarbojas.

Papildinformācija: [Pierakstīšanās problēmu novēršana](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Nevar piekļūt abonementiem**

Azure [portālā pārliecinieties,](https://portal.azure.com/)vai augšējā labajā stūrī kontā ir atlasīts pareizais Azure direktorijs.

Azure [kontu centrā pārliecinieties,](https://account.windowsazure.com/Subscriptions)vai izmantotais konts ir konta administrators.

Papildinformācija. [Problēmu novēršana saistībā ar bez abonementiem](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Nevar piekļūt norēķinu vēsturei**

Konta administratoram ir jānodrošina, lai lietotājs, kas piekļūst norēķinu informācijai, būtu pievienots Azure Active Directory kā vies lietotājs: pievienojiet vai [dzēsiet jaunu lietotāju.](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support)

Pēc tam lietotājam ir jābūt piešķirtai globālā administratora lomai: [Piešķirt lomu lietotājiem.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support)

Pēc tam lietotājam var piešķirt norēķinu piekļuvi, izmantojot RBAC politikas: [piekļuves piešķiršana norēķiniem.](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)

**Ieteiktie dokumenti**

-   [Nevaru pierakstīties, lai pārvaldītu savu Azure abonementu](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)