---
title: Problēmas ar Seamless SSO integrāciju ar lokālajām lietojumprogrammām
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
ms.openlocfilehash: 6b295f3272ba074eac3afb66f3156af7ea4065a1398a215bcb3cde5da74b198a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028299"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Problēmas ar Seamless SSO integrāciju ar lokālajām lietojumprogrammām

Lai novērstu problēmas, kas saistītas ar Seamless SSO integrāciju ar lokālajām lietojumprogrammām, rīkojieties šādi:

**Ieteicamās darbības**

1. Lai konfigurētu lokālo lietojumprogrammu vienotāi pierakstīšanās, izmantojot lietojumprogrammas starpniekserveri, skatiet rakstu **Paroles** glabātava vienotās pierakstīšanās ar [lietojumprogrammas starpniekserveri](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
1. **Lietojumprogrammas starpniekservera** problēmu novēršana : iesakām sākt pārskatīt problēmu novēršanas plūsmu, atkļūdošanas [lietojumprogrammas](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)starpniekservera savienotāja problēmas , lai noteiktu, vai lietojumprogrammas starpniekservera savienotāji ir konfigurēti pareizi. Ja joprojām rodas problēmas, veidojot savienojumu ar lietojumprogrammu, izpildiet problēmu novēršanas darbības, kas norādītās sadaļā Lietojumprogrammas starpniekservera [lietojumprogrammas atkļūdošanas problēmas.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Lai noteiktu [CORS problēmas, izmantojiet](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) tālāk norādītos pārlūkprogrammas atkļūdošanas rīkus.
    1. Palaidiet pārlūkprogrammu un pārlūkojiet līdz tīmekļa lietojumprogrammai.
    1. Nospiediet **taustiņu F12,** lai atvērtu atkļūdošanas konsoli.
    1. Mēģiniet atveidot transakciju un pārskatiet konsoles ziņojumu. CORS pārkāpumi izraisa konsoles kļūdu par izcelsmi.
    1. Dažas CORS problēmas nevar atrisināt, piemēram, kad jūsu programma novirza uz login.microsoftonline.com uz autentificēšanu un piekļuves pilnvaras derīgums beidzas. Pēc tam CORS zvans neizdodas. Risinājums šim scenārijam ir pagarināt piekļuves pilnvaras darbības laiku, lai tas nebeidzas lietotāja sesijas laikā. Papildinformāciju par to, kā to paveikt, skatiet rakstā [Konfigurējamu pilnvaru darbības ilgums Microsoft indentitāšu platforma.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)

**Ieteiktie dokumenti**

- [Kā konfigurēt vienoto pierakstīšanu lietojumprogrammas starpniekservera lietojumprogrammā](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [SAML vienotā pierakstīšanās lokālajās lietojumprogrammās ar lietojumprogrammas starpniekserveri](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Informācija par lietojumprogrammas Azure Active Directory starpniekservera CORS problēmām un to novēršana](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Kerberos ierobežoto deleģēšanas konfigurāciju problēmu novēršana lietojumprogrammas starpniekserverī](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)