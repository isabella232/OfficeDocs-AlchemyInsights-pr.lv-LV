---
title: Vienotās pierakstīšanās (Seamless Single Sign-on — SSO) konfigurēšana
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
- "9004344"
- "9004357"
- "9384"
- "9863"
ms.openlocfilehash: bd3873c2db1b8d548f81d531a8bf5747130fe761
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402274"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Vienotās pierakstīšanās (Seamless Single Sign-on — SSO) konfigurēšana

**Lietojumprogrammu konfigurēšana**

1. Iegūt vērtības no lietojumprogrammas piegādātāja. Varat manuāli ievadīt vērtības vai augšupielādēt metadatu failu, lai izvilktu lauku vērtību.
2. Daudzas programmas jau ir sākotnēji konfigurētas darbam ar Azure AD. Šīs programmas ir uzskaitītas programmu galerijā, kuras varat pārlūkot, kad pievienojat lietojumprogrammu Azure AD nomniekam. Īsās [pamācības](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) sērija palīdz veikt darbības.
3. Lai izveidotu lietojumprogrammu, kas nav galerija, varat noklikšķināt uz **pogas +** Izveidot savu lietojumprogrammu un piešķirt nosaukumu savai lietojumprogrammai.
    - Pēc noklusējuma tā atlasīs **opciju** Integrēt jebkuru citu neatrodamu lietojumprogrammu galerijā, kas ir pareizā opcija lietojumprogrammām, kas nav galerijas.
    - Kad pēc **lietojumprogrammas** nosaukuma pielikšanas iespiedīsit taustiņu Create, tiks izveidota jauna programma, kas nav galerija Enterprise.
    - Pēc tam sadaļā  Pārvaldīt šo lietojumprogrammu varat pāriet uz vienoto pierakstīšanu, un varat skatīt dažādas metodes, kā to ieviest savā vidē. 

**Seamless SSO konfigurēšana konkrētai lietojumprogrammai**

Galerijas lietojumprogrammu gadījumā atradīsit detalizētus norādījumus. Lai piekļūtu darbībām, varat pārlūkot visu programmu konfigurācijas apmācību sarakstu [saaS programmu konfigurācijas apmācībās.](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)

**SamL SSO konfigurēšana**

1. [Īsā pamācība: SAML vienotās pierakstīšanās (SSO) iestatīšana lietojumprogrammai Azure Active Directory (Azure AD) nomniekā.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)
2. Papildinformāciju par SAML vienotās pierakstīšanās opciju skatiet rakstā [SAML vienotās pierakstīšanās izpratne.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on)
3. Lai uzzinātu par SAML 2.0 autentifikācijas pieprasījumiem un atbildēm, ko Azure Active Directory (Azure AD) atbalsta single Sign-On (SSO), skatiet sadaļu [Single Sign-On SAML protokols.](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
4. Lai uzzinātu, kā izveidot un konfigurēt SAML vienotās pierakstīšanās (SSO) jūsu programmai pakalpojumā Azure Active Directory (Azure AD), izmantojot Microsoft Graph API, skatiet rakstu SAML vienotās pierakstīšanās konfigurēšana lietojumprogrammai, izmantojot [Microsoft Graph API.](https://docs.microsoft.com/graph/application-saml-sso-configure-api)
5. Lai uzzinātu, kā Azure AD izmanto SAML protokolu, skatiet rakstu [Kā Microsoft identitātes platforma izmanto SAML protokolu.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference)

**Pilnvaru un prasību konfigurēšana**

1. [How to: customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).
2. Lai uzzinātu, kā konfigurēt prasības, izmantojot PowerShell, skatiet rakstu Kā: pielāgot prasības, kas izlaistas marķieriem konkrētai lietojumprogrammai nomniekā [(priekšskatījums).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
3. Lai uzzinātu, kā konfigurēt neobligātās prasības, [skatiet rakstu Kā: norādiet papildu prasības uz savu lietojumprogrammu.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
4. Lai uzzinātu, kā izmantot direktorija shēmas paplašinājuma atribūtus lietotāju datu sūtīšanai uz lietojumprogrammām marķieru prasības, skatiet rakstu [Direktorija shēmas paplašinājuma atribūtu izmantošana prasības.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions)
5. Lai uzzinātu, kā konfigurēt pilnvaru darbības laikus, skatiet rakstu Konfigurējamus pilnvaru darbības laikus Microsoft identitātes platformā [(priekšskatījums).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
6. [Pilnvaru darbības politiku konfigurēšana (priekšskatījums)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) — šajā rakstā ir aprakstītas kopējās politikas scenārijs, kas var palīdzēt noteikt jaunas kārtulas pilnvaru darbības laikā. Šajā piemērā jūs uzzināsit, kā izveidot politiku, kas lietotājiem pieprasa biežāk autentifikāciju tīmekļa lietojumprogrammā.

**SSO konfigurācijas problēmu novēršana**

- Bieži uzdotie jautājumi par Azure Active Directory Seamless Single Sign-On (Seamless SSO), skatiet [rakstā Azure Active Directory Seamless Single Sign-On: bieži uzdotie jautājumi.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq)
- Lai novērstu informāciju par bieži sastopamām problēmām saistībā ar Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO), skatiet rakstu Azure Active Directory Vienotās [pierakstīšanās problēmu novēršana.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso)
