---
title: Problēmas ar token prasībām un atribūtiem
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
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035965"
---
# <a name="issues-with-token-claims-and-attributes"></a>Problēmas ar token prasībām un atribūtiem

**Apliecinājuma prasību atjaunināšana, konfigurēšana un noņemšana**

1. Izmantojot Azure Active Directory (Azure AD), varat [pielāgot pieprasījuma tipu lomai](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) , kas saņemta pēc tam, kad esat autorizējis programmu.
2. Lietojumprogrammu izstrādātāji var izmantot neobligātas prasības to Azure AD lietojumprogrammās, lai norādītu, kuras prasības tās vēlas piešķirt. Lai iegūtu papildinformāciju, skatiet rakstu [kā sniegt neobligātus pieprasījumus savai programmai](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
3. [Konfigurējiet grupu pieprasījumus pakalpojumam Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. Ja lietojumprogrammā izmantojat nemanāmu vienoto pierakstīšanos, skatiet rakstu [SAML pilnvarā izsniegto prasību pielāgošana Enterprise lietojumprogrammām](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).

**Pretenziju atribūtu kartēšana**

1. Lai konfigurētu pieprasījumu kartēšanas politikas izmantošanu, izmantojot PowerShell, skatiet rakstu kā noteiktās [programmas nomniekā (priekšskatījums) pielāgotās prasības](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
2. Direktorija shēmas paplašinājuma atribūti nodrošina veidu, kā glabāt papildu datus Azure Active Directory lietotāju objektos un citos direktorija objektos, piemēram, grupās, nomnieka informācijā, pakalpojumu principālos. Tikai lietotāja objektu paplašinājuma atribūtus var izmantot, lai izceltu lietojumprogrammas. [Direktorija shēmas paplašinājuma atribūtu izmantošana prasībās](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) ir aprakstīts, kā izmantot direktorija shēmas paplašinājuma atribūtus, lai sūtītu lietotāja datus lietojumprogrammām ar marķiera prasībām.

Papildinformāciju par marķierierīces prasībām skatiet rakstā:

- [Prasības Access marķierierīcēs](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Prasības id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Norādes](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) , ko var sagaidīt ID marķierierīcēs un piekļuves marķierierīcēs, ko izsniedz AZURE ad B2C
- [SAML marķiera norādes](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
