---
title: Viesa lietotāju problēmu novēršana
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
ms.openlocfilehash: 0f2a10b918fee067b167ab58ac2544a89e0c8ea1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901171"
---
# <a name="troubleshoot-guest-user-issues"></a>Viesa lietotāju problēmu novēršana

1. Norādījumus par viesu piekļuves lietojumprogrammām pārvaldību skatiet rakstā [viesu piekļuves pārvaldība, izmantojot AZURE ad Access Recenzijas](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews).
1. [Vieslietotāju pievienošana direktorijam Azure portālā](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal): šajā Quickstart, jūs pievienosit jaunu vieslietotāju savam Azure AD direktorijam, izmantojot Azure portālu, nosūtot uzaicinājumu, un Uzziniet, kā izskatās vieslietotāja uzaicinājuma izpirkšanas process.
1. [Vieslietotāja pievienošana, izmantojot PowerShell](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell): šajā Quickstart, jūs izmantosit komandu New-AzureADMSInvitation, lai pievienotu vienu vieslietotāju savam Azure nomniekam.
1. Lai uzzinātu, kā lietotājiem un grupām piešķirt uzņēmuma lietojumprogrammas Azure Active Directory (Azure AD), vai nu Azure portālā vai izmantojot PowerShell, skatiet rakstu [lietotāja piešķirtās programmas Azure Active Directory pārvaldība](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal). 
1. Azure Active Directory (Azure AD) B2B sadarbība darbojas ar lielāko daļu programmu, kas ir integrētas ar Azure AD. Šajā [rakstā](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)ir sniegti norādījumi par to, kā konfigurēt dažas populārās Saas lietojumprogrammas AZURE ad B2B lietošanai.
1. Kā organizācija, kas izmanto Azure Active Directory (Azure AD) B2B sadarbības iespējas, lai uzaicinātu vieslietotājus no partnera organizācijām uz jūsu Azure AD, jūs tagad varat nodrošināt šiem B2B lietotājiem piekļuvi lokālās lietojumprogrammas. Šīs lokālās lietojumprogrammas var izmantot SAML autentifikāciju vai integrētu Windows autentifikāciju (IWA) ar Kerberos ierobežotu deleģēšanu (KCD). Lai iegūtu papildinformāciju, skatiet rakstu [B2B lietotājiem piešķirt AZURE ad piekļuvi savām](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)lokālajām lietojumprogrammām.
1. Uzziniet, kā [piešķirt lokāli pārvaldītu partnera kontu piekļuvi mākoņa resursiem, izmantojot AZURE ad B2B sadarbību](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud).