---
title: Problēmas ar viengabala SSO integrāciju ar manām lokālajām lietojumprogrammām
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/13/2021
ms.locfileid: "49868716"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Problēmas ar viengabala SSO integrāciju ar manām lokālajām lietojumprogrammām

Lai novērstu problēmas, kas saistītas ar viengabala SSO integrāciju ar lokālajām lietojumprogrammām, veiciet tālāk norādītās darbības.

**Ieteicamās darbības**

1. Lai konfigurētu **lokālo lietojumprogrammu** **vienotās pierakstīšanās lietošanai, izmantojot lietojumprogrammu starpniekserveri**, skatiet rakstu [paroļu velves izveide vienotā pierakstīšanās ar lietojumprogrammas starpniekserveri](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
1. **Lietojumprogrammas starpniekservera problēmu novēršana**: iesakām sākt ar problēmu novēršanas plūsmu pārskatīšanu, [atkļūdošanas lietojumprogrammas starpniekservera savienotāja problēmas](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), lai noteiktu, vai lietojumprogrammas starpniekservera savienotāji ir konfigurēti pareizi. Ja joprojām rodas problēmas, veidojot savienojumu ar lietojumprogrammu, veiciet problēmu novēršanas darbības sadaļā [atkļūdošanas lietojumprogrammas starpniekservera problēmas](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). Varat [IDENTIFICĒT CORS problēmas](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) , izmantojot tālāk norādītos pārlūkprogrammas atkļūdošanas rīkus.
    1. Palaidiet pārlūkprogrammu un pārlūkojiet līdz tīmekļa programmai.
    1. Nospiediet taustiņu **F12** , lai atvērtu atkļūdošanas konsoli.
    1. Mēģināt reproducēt transakciju un pārskatīt konsoles ziņojumu. CORS pārkāpums izveido konsoles kļūdu par izcelsmi.
    1. Dažas CORS problēmas nevar atrisināt, piemēram, kad lietojumprogramma novirza uz login.microsoftonline.com, lai autentificētu, un piekļuves pilnvaras derīguma termiņš beigsies. CORS pēc tam neizdosies. Risinājums šajā scenārijā ir pagarināt piekļuves marķiera kalpošanas laiku, lai neļautu tam beigties lietotāja sesijas laikā. Papildinformāciju par to, kā to paveikt, skatiet rakstā [konfigurējamas marķierierīces ilgumus Microsoft identitātes platformā](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

**Ieteicamie dokumenti**

- [Kā konfigurēt vienoto pierakstīšanos lietojumprogrammas starpniekservera lietojumprogrammā](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [SAML Single Sign-On lokālās lietojumprogrammas, izmantojot lietojumprogrammas starpniekserveri](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Azure Active Directory lietojumprogrammas starpniekservera CORS problēmu izprašana un risināšana](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Problēmu novēršana saistībā ar Kerberos ierobežotu deleģēšanas konfigurāciju lietojumprogrammas starpniekserverim](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)