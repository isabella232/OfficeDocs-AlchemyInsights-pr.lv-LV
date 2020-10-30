---
title: Abonementa piekļuve
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
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807436"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Nevar pierakstīties Azure ar pārlūkprogrammu saistītu problēmu dēļ (pārlūkprogramma uzkaras, turpina vērpšanas, netiek ielādēts utt.)

Iespējams, jūs ietekmēs pārtraukums. Lūdzu, pārbaudiet, vai pastāv nepārtraukts pārtraukums: [Azure darbspējas statuss](https://status.azure.com/status/history/).

Lūdzu, atsakieties no visām aktīvajām Azure sesijām. Startējiet tīmekļa pārlūkprogrammas privātu vai inkognito režīmu.

Varat arī mēģināt atsvaidzināt pārlūkprogrammu, izmantot citu pārlūkprogrammu, dzēst kešatmiņas sīkfailus, ja tas nedarbojas.

Papildinformācija: [pierakstīšanās problēmu novēršana](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Nevar piekļūt abonementiem**

[Azure portālā](https://portal.azure.com/)pārliecinieties, vai no konta augšpusē pa labi ir atlasīts pareizs Azure direktorijs.

[Azure kontu centrā](https://account.windowsazure.com/Subscriptions)pārliecinieties, vai izmantotais konts ir konta administrators.

Papildinformācija: [problēmu novēršana nav atrasti](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Nevar piekļūt norēķinu vēsturei**

Konta administratoram ir jāpārliecinās, ka lietotājs piekļūst norēķinu informācijai, Azure Active Directory tiek pievienots kā vieslietotājs: [pievienojiet vai dzēsiet jaunu lietotāju](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

Pēc tam lietotājam ir jāpiešķir globālā administratora loma: [piešķirt lomai lietotājiem](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Ziņas izlikšana lietotājam var piešķirt norēķinu piekļuvi, izmantojot RBAC politikas: [piešķirt piekļuvi norēķiniem](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**Ieteicamie dokumenti**

-   [Nevaru pierakstīties, lai pārvaldītu savu Azure abonementu](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)