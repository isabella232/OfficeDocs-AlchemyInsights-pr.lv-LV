---
title: Problēmas ar marķieru prasībām un atribūtiem
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
- "9004347"
- "7761"
ms.openlocfilehash: 0c9827ee312d6b236c86f5a2973fa61fdc78c49b8565dd4ceb41f9a3a48140bc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012891"
---
# <a name="issues-with-token-claims-and-attributes"></a>Problēmas ar marķieru prasībām un atribūtiem

**Marķiera prasības atjaunināšana, konfigurēšana vai noņemšana**

1. Izmantojot Azure Active Directory (Azure AD), varat [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) pielāgot pieprasāmās informācijas tipu lomas pieprasāmā summai atbildes pilnvarai, ko saņemat pēc lietojumprogrammas autorizētšanas.
2. Lietojumprogrammu izstrādātāji savās Azure AD lietojumprogrammās var izmantot papildu prasības, lai norādītu, kuras prasības viņi vēlas savā lietojumprogrammā nosūtītos marķieros. Papildinformāciju skatiet rakstā [Papildu prasību par programmu sniegšanas informācija.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
3. [Konfigurējiet grupas prasības lietojumprogrammām, izmantojot Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. Ja savā lietojumprogrammā izmantojat Seamless Single Sign-on, skatiet rakstu SAML marķiera enterprise lietojumprogrammām [izdoto prasību pielāgošana.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)

**Claims Attribute Mapping**

1. Lai konfigurētu prasību kartēšanas politiku, izmantojot PowerShell, skatiet rakstu Pielāgot prasības, kas izlaistas marķieros konkrētai lietojumprogrammai [nomniekā (priekšskatījums).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
2. Direktorija shēmas paplašinājuma atribūti nodrošina veidu, kā lietotāja objektos un Azure Active Directory citos direktorija objektos, piemēram, grupās, nomnieka detaļās, pakalpojumā saglabāt papildu datus. Lietojumprogrammu prasību izšanai var izmantot tikai paplašinājuma atribūtus lietotāju objektos. [Direktorija shēmas paplašinājuma atribūtu izmantošana](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) claimsos apraksta, kā izmantot direktorija shēmas paplašinājuma atribūtus lietotāju datu sūtīšanai uz lietojumprogrammām marķiera prasības.

Papildinformāciju par marķieru prasībām skatiet šeit:

- [Claims in access tokens](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Claims in an id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) that you can expect in ID tokens and access tokens issued by Azure AD B2C
- [SAML marķiera prasības atsauce](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
