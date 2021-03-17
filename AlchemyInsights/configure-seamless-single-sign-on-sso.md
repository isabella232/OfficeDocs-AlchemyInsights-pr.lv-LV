---
title: Netraucētas vienotās pierakstīšanās (SSO) konfigurēšana
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
- "9384"
ms.openlocfilehash: 32790b23547de36cd2864e85ebae67f54ad91707
ms.sourcegitcommit: 309b9f3e6e2ff622f95bb860d337d2c05b7bbe54
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/15/2021
ms.locfileid: "50841536"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Netraucētas vienotās pierakstīšanās (SSO) konfigurēšana

**Lietojumprogrammu konfigurēšana**

1. Jums ir jāiegūst vērtības no lietojumprogrammas piegādātāja. Varat manuāli ievadīt vērtības vai augšupielādēt metadatu failu, lai izvilktu lauku vērtību.
2. Daudzas programmas jau ir iepriekš konfigurētas darbam ar Azure AD. Šīs lietojumprogrammas ir norādītas to lietojumprogrammu galerijā, kuras varat pārlūkot, pievienojot programmai Azure AD nomniekam. [Quickstart Series](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) palīdz veikt šo procesu.
3. Lai izveidotu lietojumprogrammu, kas nav galerija, varat noklikšķināt uz **+ izveidot savu lietojumprogrammas** pogu un piešķirt savai lietojumprogrammai nosaukumu.
    - Pēc noklusējuma tiks atlasīts **integrēt jebkuru citu lietojumprogrammu, kuru neatrodat galerijā,** kas ir atbilstoša opcijai, kas nav galerijas lietojumprogrammas.
    - Kad būsit noklikšķinājis uz **izveidot** pēc tam, kad būsit iesniedzis lietojumprogrammas nosaukumu, tiks izveidota jauna ne galerijas uzņēmuma lietojumprogramma.
    - Pēc tam varat pāriet uz **vienoto pierakstīšanos** zem šīs lietojumprogrammas **pārvaldības** un jūs varēsit redzēt dažādas metodes, lai to īstenotu savā vidē.

**Nemanāma SSO konfigurēšana noteiktai lietojumprogrammai**

Galerijā ietvertās programmas atradīsit detalizētus detalizētos norādījumus. Lai piekļūtu šīm darbībām, varat pārlūkot sarakstu ar visām programmu konfigurācijas apmācībām vietnē [Saas lietojumprogrammas konfigurācija](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list).

**SAML SSO konfigurēšana**

1. [Quickstart: iestatiet SAML vienotās pierakstīšanās (SSO) lietojumprogrammai Azure Active Directory (AZURE AD) nomniekā](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso).
2. Lai iegūtu papildinformāciju par vienotās pierakstīšanās opciju SAML, skatiet rakstu [SAML vienotās pierakstīšanās izpratne](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on).
3. Lai uzzinātu par SAML 2,0 autentifikācijas pieprasījumiem un atbildēm, ka Azure Active Directory (Azure AD) atbalsta viena Sign-On (SSO), skatiet rakstu [single Sign-On SAML protokols](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol).
4. Lai uzzinātu, kā izveidot un konfigurēt SAML vienotās pierakstīšanās (SSO) jūsu lietojumprogrammā Azure Active Directory (Azure AD), izmantojot Microsoft Graph API, skatiet rakstu [SAML vienotās pierakstīšanās konfigurēšana, izmantojot Microsoft GRAPH API](https://docs.microsoft.com/graph/application-saml-sso-configure-api).
5. Lai uzzinātu, kā Azure AD izmanto SAML protokolu, skatiet rakstu [kā Microsoft Identity Platform izmanto SAML protokolu](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference).

**Tokens un prasību konfigurēšana**

1. [Kā: pielāgot prasības, kas emitētas SAML pilnvarā uzņēmumiem](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).
2. Lai uzzinātu, kā konfigurēt pretenzijas, izmantojot PowerShell, skatiet rakstu [kā veikt tālāk norādītās darbības](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
3. Lai uzzinātu, kā konfigurēt papildu prasības, skatiet rakstu [kā: sniegt neobligātus pieprasījumus savai programmai](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
4. Lai uzzinātu, kā izmantot direktorija shēmas paplašinājuma atribūtus lietotāju datu sūtīšanai uz lietojumprogrammām, izmantojot pilnvaras, skatiet rakstu [direktorija shēmas paplašinājuma atribūtu izmantošana prasībās](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions).
5. Lai uzzinātu, kā konfigurēt marķierierīces ilgumu, skatiet rakstu [konfigurējamas marķierierīces kalpošanas laiks Microsoft identitātes platformā (priekšskatījums)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
6. [Token Lifetime politikas (priekšskatījums) konfigurēšana](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) -šajā rakstā ir izklāstīts kopējais politikas scenārijs, kas var palīdzēt uzlikt jaunus noteikumus attiecībā uz marķierierīces kalpošanas laiku. Šajā piemērā uzzināsit, kā izveidot politiku, kas lietotājiem ir jāautentificē biežāk savā tīmekļa lietojumprogrammā.

**SSO konfigurācijas problēmu novēršana**

- Lai saņemtu atbildes uz bieži uzdotiem jautājumiem par Azure Active Directory nevainojamu atsevišķu Sign-On (viengabala SSO), skatiet rakstu [Azure Active Directory vienotā pierakstīšanās: bieži uzdotie jautājumi](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq).
- Lai iegūtu informāciju par biežāk sastopamajām problēmām attiecībā uz Azure Active Directory (Azure AD) viengabala Single Sign-On (viengabala SSO), skatiet rakstu [problēmu novēršana Azure Active Directory nemanāma vienotā pierakstīšanās](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso).
