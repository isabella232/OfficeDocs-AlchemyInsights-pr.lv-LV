---
title: SSO savienojuma problēmas
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
- "9004357"
- "7810"
ms.openlocfilehash: 8fb93bc40c6cd5a7c0e3d259fe3be8d1bab3187dd5aa023eb49977555fd930de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084353"
---
# <a name="sso-connection-issues"></a>SSO savienojuma problēmas

1. Izpildiet [īsās pamācības norādījumus: lietojumprogrammas rokasgrāmatas rekvizītu](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) konfigurēšana, lai konfigurētu programmu.
2. Atkarībā no izvēlētās [lietojumprogrammas un vienotās](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) pierakstīšanās opcijas, izpildiet tālāk norādītās darbības.
    - Lai konfigurētu lokālo lietojumprogrammu **SAML** **vienotās** pierakstīšanās vajadzībām, skatiet rakstu SAML vienotā pierakstīšanās lokālajās lietojumprogrammās ar [lietojumprogrammas starpniekserveri.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
    - Lai konfigurētu **mākoņa** **lietojumprogrammu vienotās pierakstīšanās** ar paroli gadījumā, skatiet rakstu [Vienotās pierakstīšanās ar paroli konfigurēšana.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)
    - Lai konfigurētu lokālo lietojumprogrammu vienotāi pierakstīšanās, izmantojot lietojumprogrammas starpniekserveri, skatiet rakstu **Paroles** glabātava vienotās pierakstīšanās ar [lietojumprogrammas starpniekserveri](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
3. **Lietojumprogrammas starpniekservera** problēmu novēršana : ieteicams sākt ar pārskatu par problēmu [novēršanu,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)lietojumprogrammas starpniekservera savienotāja atkļūdošanas problēmām , lai noteiktu, vai lietojumprogrammas starpniekservera savienotāji ir konfigurēti pareizi. Ja joprojām rodas problēmas, veidojot savienojumu ar lietojumprogrammu, izpildiet problēmu novēršanas plūsmu sadaļā Lietojumprogrammas starpniekservera [lietojumprogrammas atkļūdošanas problēmas.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Lai noteiktu [CORS problēmas, izmantojiet](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) pārlūkprogrammas atkļūdošanas rīkus.
    - Palaidiet pārlūkprogrammu un pārlūkojiet līdz tīmekļa lietojumprogrammai.
    - Nospiediet **taustiņu F12,** lai atvērtu atkļūdošanas konsoli.
    - Mēģiniet atveidot transakciju un pārskatiet konsoles ziņojumu. CORS pārkāpumi izraisa konsoles kļūdu par izcelsmi.
    - Dažas CORS problēmas nevar atrisināt, piemēram, kad jūsu programma novirza uz login.microsoft.com uz autentificēšanu un piekļuves pilnvaras derīgums beidzas. Pēc tam CORS zvans neizdodas. Risinājums šim scenārijam ir pagarināt piekļuves pilnvaras darbības laiku, lai tas nebeidzas lietotāja sesijas laikā. Papildinformāciju par to, kā to paveikt, skatiet rakstā [Konfigurējamu pilnvaru darbības ilgums Microsoft indentitāšu platforma.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
4. **SAML vienotās pierakstīšanās** problēmu novēršana: iesakām pārbaudīt Problēmas ar pierakstīšanos [SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)vienotās pierakstīšanās konfigurētās programmās , lai atrastu risinājumus problēmām, ar kurām visdrīzāk saskarsieties.
5. **Ar paroli pamatotas vienotās pierakstīšanās** problēmu novēršana: iesakām pārbaudīt novērst ar paroli balstītu vienoto pierakstīšanos pakalpojumā [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso), lai atrastu risinājumus problēmām, ar kurām visdrīzāk saskarsieties.
6. Informāciju par savienojuma problēmām VPN izmantošanas laikā skatiet rakstā Vienotās pierakstīšanās (single sign on — [SSO) izmantošana VPN un Wi-Fi savienojumos.](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)
