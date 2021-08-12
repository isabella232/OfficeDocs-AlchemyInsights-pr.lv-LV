---
title: Viesu lietotāju problēmu novēršana
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004358"
- "7822"
ms.openlocfilehash: 9e6030919721b4c0805a26ca45d365f31d88894e86ea08225f47576e7d152047
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939386"
---
# <a name="troubleshoot-guest-user-issues"></a>Viesu lietotāju problēmu novēršana

1. Norādījumus par viesu piekļuves lietojumprogrammām pārvaldību skatiet rakstā [Viesu piekļuves pārvaldība, izmantojot Azure AD piekļuves atsauksmes.](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews)
1. [Viesa lietotāju](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)pievienošana direktorijam Azure portālā: šajā ātrajā pamācībā savam Azure AD direktorijam pievienosit jaunu vies lietotāju, izmantojot Azure portālu, nosūtīsit uzaicinājumu un apskatīsit, kā izskatās viesa lietotāja uzaicinājuma izpirkšanas process.
1. [Viesa lietotāja pievienošana, izmantojot PowerShell:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell)šajā ātrajā pamācībā izmantosit komandu New-AzureADMSInvitation, lai Azure nomniekam pievienotu vienu viesa lietotāju.
1. Lai uzzinātu, kā piešķirt lietotājus un grupas uzņēmuma lietojumprogrammām programmā Azure Active Directory (Azure AD) Azure portālā vai izmantojot PowerShell, skatiet rakstu Lietotāju piešķires pārvaldība lietojumprogrammai [programmā Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal) 
1. Azure Active Directory (Azure AD) B2B sadarbojas ar lielāko daļu lietojumprogrammu, kas ir integrētas azure AD. Šajā rakstā [ir](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)sniegti norādījumi dažu populāru SaaS programmu konfigurēšanai izmantošanai ar Azure AD B2B.
1. Kā organizācija, kas izmanto Azure Active Directory (Azure AD) B2B sadarbības iespējas, lai uzaicinātu viesa lietotājus no partneru organizācijām jūsu Azure AD, tagad varat nodrošināt šiem B2B lietotājiem piekļuvi lokālajām programmām. Šīs lokālās programmas var izmantot SAML autentifikāciju vai integrēto autentifikāciju Windows (IWA) ar Kerberos ierobežoto deleģēšanu (Integrated Windows Authentication — IWA). Papildinformāciju skatiet [rakstā B2B lietotāju piešķiršana azure AD piekļuve lokālajām lietojumprogrammām.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)
1. Uzziniet, [kā lokāli pārvaldītiem partneru kontiem piešķirt piekļuvi mākoņresursiem, izmantojot Azure AD B2B sadarbības iespējas.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)