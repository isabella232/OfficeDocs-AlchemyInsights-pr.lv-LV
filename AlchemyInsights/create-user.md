---
title: Izveidot lietotāju
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
ms.openlocfilehash: 742ff857141d08031302fdcff7e49b3eef90e0f7
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744977"
---
# <a name="create-user"></a>Izveidot lietotāju

**PAZIŅOJUMU**

- Tīmekļa [skata pierakstīšanās atbalsts no Google, sākot ar 4. janvāri, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) . Pārbaudiet, vai jūsu lietojumprogrammas var ietekmēt, ievērojot [Google norādījumus](https://go.microsoft.com/fwlink/?linkid=2157323) par saderību testēšanā.
- Pierakstoties lietotājiem ar patērētāju Google kontiem, noteikti izmantojiet sistēmas tīmekļa skatu vai sistēmas pārlūkprogrammu. Papildinformāciju skatiet rakstā problēmas, [pierakstoties lietojumprogrammā (-as), izmantojot tikai Chrome pārlūkprogrammu](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).

**Nevaru izveidot jaunu lietotāju savā Azure AD direktorijā**

1. Pārliecinieties, vai esat autorizēts izveidot jaunu standarta lietotāju. Azure Active Directory (AD) tikai globālā administratora vai lietotāja administratora loma var izveidot jaunu standarta lietotāju. Ja neesat kādā no šīm lomām, lūdziet administratoram pievienot jūs kādai no šīm lomām vai izveidot jaunu lietotāja kontu.
1. Pārliecinieties, vai lietotājvārds ir domēnā, kas ir verificēts Azure AD. Ja Azure AD nav pārbaudīti pielāgoti domēnu nosaukumi, varat izmantot Azure AD sākotnējo domēnu, kas beidzas ar *. onmicrosoft.com.
1. Pārliecinieties, vai lietotājvārds ir domēnā, kas nav Azure AD integrētās reklāmas no lokālās reklāmas. Lietotāji nevar pievienot mākonī ar domēnu nosaukumiem, kas tiek apvienoti no lokālās atrašanās vietas.
1. Pārliecinieties, vai nevienam lietotājam vai kontaktpersonai jau ir lietotājvārds, ko vēlaties piešķirt jaunajam lietotājam. Lietotāju nosaukumiem ir jābūt unikāliem visā Azure AD.
1. Skatiet [Azure AD lomas un administratorus](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) par savu Azure AD.
1. Skatiet Azure AD [domēnu nosaukumus](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) .
1. Pārskatiet [audita žurnālus](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) , lai skatītu detalizētāku informāciju par nesen izveidotu vai izdzēstu lietotāju, piemēram, kurš veica darbību, un kad.
1. Lai iegūtu papildinformāciju par jaunu lietotāju pievienošanu, skatiet sadaļu [debeszils portāla izmantošana, lai izveidotu jaunu lietotāju AZURE ad](/azure/active-directory/active-directory-users-create-azure-portal).
1. [AZURE ad administratīvās lomas](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles): administratora lomu atļaujas Azure Active Directory
1. Varat arī [izmantot AZURE ad PowerShell, lai izveidotu jaunu lietotāju](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).
