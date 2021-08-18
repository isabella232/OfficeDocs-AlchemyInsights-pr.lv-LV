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
ms.openlocfilehash: d86b2dd6d7915f0698cf950cd57f1065cde22219284edbbc0e64f3a5e69ff252
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896722"
---
# <a name="create-user"></a>Lietotāja izveide

**PAZIŅOJUMS:**

- Google tīmekļa skata pierakstīšanās atbalsta noilgums no [2021. gada 4. janvāra](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) Pārbaudiet, vai jūsu programmas var ietekmēt [Google norādījumi par](https://go.microsoft.com/fwlink/?linkid=2157323) testēšanu saderību.
- Pārliecinieties, vai izmantojat sistēmas tīmekļa skatu vai sistēmas pārlūkprogrammu, pierakstoties lietotāju Google patērētāju kontos. Papildinformāciju skatiet rakstā [Problēmas ar pierakstīšanos lietojumprogrammās, kas izmanto tikai pārlūkprogrammu Chrome.](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)

**Es nevaru izveidot jaunu lietotāju savā Azure AD direktorijā**

1. Pārliecinieties, vai esat pilnvarots izveidot jaunu standarta lietotāju. Jaunu standarta lietotāju var izveidot tikai globālā administratora vai Azure Active Directory administratora loma Azure Active Directory (AD). Ja jums nav šīs lomas, lūdziet administratoram jūs pievienot kādai no šīm lomām vai izveidot jaunu lietotāja kontu jūsu vietā.
1. Pārliecinieties, vai lietotājvārds ir domēnā, kas ir verificēts jūsu Azure AD. Ja jūsu Azure AD nav neviena verificēta pielāgoto domēnu nosaukumu, varat izmantot savu Azure AD sākotnējo domēnu, kas beidzas ar *.onmicrosoft.com.
1. Pārliecinieties, vai lietotājvārds ir domēnā, kas nav federēts uz Azure AD no jūsu lokālā AD. Lietotājus nevar pievienot mākonī ar domēnu nosaukumiem, kas ir federatīvi no lokāla domēna.
1. Pārliecinieties, vai nevienam citam lietotājam vai kontaktpersonai nav lietotājvārda, ko vēlaties piešķirt jaunajam lietotājam. Lietotājvārdiem ir jābūt unikāliem visā Azure AD.
1. Skatiet [Azure AD lomas un administratorus](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) savam Azure AD.
1. Skatiet [sava](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) Azure AD domēnu nosaukumus.
1. Pārskatiet [audita žurnālus,](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) lai skatītu detalizētu informāciju par nesen izveidotu vai izdzēstu lietotāju kā personu, kas veica šo darbību un kad.
1. Papildinformāciju par jaunu lietotāju [pievienošanu skatiet rakstā Azure portāla izmantošana, lai izveidotu jaunu lietotāju savā Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-users-create-azure-portal)
1. [Azure AD administratīvās lomas:](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles)Administratora lomu atļaujas Azure Active Directory
1. Varat arī izmantot [Azure AD PowerShell, lai izveidotu jaunu lietotāju.](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)
