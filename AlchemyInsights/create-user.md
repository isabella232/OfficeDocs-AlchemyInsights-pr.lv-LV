---
title: Lietotāja izveide
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: 800baae2d748708d8cb7a5fb0e73fce5dcf455cb
ms.sourcegitcommit: 2d617ae59eed0ce8b571339ceefce6473c03b94c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/19/2021
ms.locfileid: "52569738"
---
# <a name="create-user"></a>Lietotāja izveide

**PAZIŅOJUMS:**

- Google tīmekļa skata pierakstīšanās atbalsta noilgums, sākot no [2021. gada 4. janvāra.](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) Pārbaudiet, vai jūsu programmas var ietekmēt [Google norādījumi par](https://go.microsoft.com/fwlink/?linkid=2157323) testēšanu saderību.
- Pārliecinieties, vai izmantojat sistēmas tīmekļa skatu vai sistēmas pārlūkprogrammu, pierakstoties lietotāju Google patērētāju kontos. Papildinformāciju skatiet rakstā [Problēmas ar pierakstīšanos lietojumprogrammās, kas izmanto tikai pārlūkprogrammu Chrome.](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)

**Es nevaru izveidot jaunu lietotāju savā Azure AD direktorijā**

1. Pārliecinieties, vai esat pilnvarots izveidot jaunu standarta lietotāju. Jaunu standarta lietotāju var izveidot tikai globālā administratora vai Azure Active Directory administratora loma programmā Azure Active Directory (AD). Ja jums nav šīs lomas, lūdziet administratoram jūs pievienot kādai no šīm lomām vai izveidot jaunu lietotāja kontu jūsu vietā.
1. Pārliecinieties, vai lietotājvārds ir domēnā, kas ir verificēts jūsu Azure AD. Ja jūsu Azure AD nav neviena verificēta pielāgoto domēnu nosaukumu, varat izmantot savu Azure AD sākotnējo domēnu, kas beidzas ar *.onmicrosoft.com.
1. Pārliecinieties, vai lietotājvārds ir domēnā, kas nav federēts uz Azure AD no jūsu lokālā AD. Lietotājus nevar pievienot mākonī ar domēnu nosaukumiem, kas ir federatīvi no lokāla domēna.
1. Pārliecinieties, vai nevienam citam lietotājam vai kontaktpersonai nav lietotājvārda, ko vēlaties piešķirt jaunajam lietotājam. Lietotājvārdiem ir jābūt unikāliem visā Azure AD.
1. Skatiet [Azure AD lomas un administratorus](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) savam Azure AD.
1. Skatiet [sava](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) Azure AD domēnu nosaukumus.
1. Pārskatiet [audita žurnālus,](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) lai skatītu detalizētu informāciju par nesen izveidotu vai izdzēstu lietotāju kā personu, kas veica šo darbību un kad.
1. Papildinformāciju par jaunu lietotāju [pievienošanu skatiet rakstā Azure portāla izmantošana, lai izveidotu jaunu lietotāju savā Azure AD.](/azure/active-directory/active-directory-users-create-azure-portal)
1. [Azure AD administratīvās lomas:](/azure/active-directory/active-directory-assign-admin-roles)Administratora lomu atļaujas Azure Active Directory
1. Varat arī izmantot [Azure AD PowerShell, lai izveidotu jaunu lietotāju.](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)
