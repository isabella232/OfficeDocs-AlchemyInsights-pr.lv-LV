---
title: API atļaujas un piekrišanas process
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
- "9004345"
- "9200"
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/26/2021
ms.locfileid: "51404873"
---
# <a name="api-permissions-and-consent-process"></a>API atļaujas un piekrišanas process

Lai jūsu lietojumprogramma varētu piekļūt datiem programmā Microsoft Graph, lietotājam vai administratoram tā ir jāpiešķir pareizās atļaujas, izmantojot piekrišanas procesu. [Microsoft Graph atļauju atsaucē ir](https://docs.microsoft.com/graph/permissions-reference) uzskaitītas atļaujas, kas saistītas ar katru galveno Microsoft Graph API kopu. Tajā arī sniegti norādījumi par atļauju lietošanu.

**Pakalpojuma pamatsummas iestatīšana vai atjaunināšana**

- [Create serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) — šajā rakstā paskaidrots, kā izveidot jaunu servicePrincipal objektu.
- [Azure AD](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) lietojumprogrammas & pamatnosauka izveide portālā — šajā rakstā paskaidrots, kā izveidot jaunu Azure Active Directory (Azure AD) lietojumprogrammu un pakalpojuma galveno nosaukumu, ko var izmantot ar lomu piekļuves vadību.
- [Lietojumprogrammas &](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) pakalpojuma pamatnosaucību pakalpojumā Azure AD — šajā rakstā aprakstīta lietojumprogrammu reģistrēšana, lietojumprogrammu objekti un pakalpojuma pamatsumma pakalpojumā Azure Active Directory: kas tās ir, kā tās tiek izmantotas un kā tās ir saistītas savā starpā.

**Pievienot vai atjaunināt lietojumprogrammu reģistrāciju un sniegt administratora piekrišanu**

- [Lietojumprogrammas reģistrācijas](https://docs.microsoft.com/graph/api/application-post-applications) izveide — šajā rakstā paskaidrots, kā izveidot jaunu lietojumprogrammas objektu.
- [Atjaunināt lietojumprogrammas reģistrāciju — API](https://docs.microsoft.com/graph/api/application-update) atļaujas — šajā rakstā aprakstīts, kā atjaunināt lietojumprogrammas objekta rekvizītus.
- [Sniedziet administratora piekrišanu](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) — administratora piekrišanai un vispār piekrišanai mēs pieprasām, lai administrators sniegtu atļauju tieši.
- [RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) — lomu pārvaldības konteiners vienotām lomu definīcijām un lomu uzdevumiem Microsoft 365 RBAC pakalpojumu sniedzējiem, kas vienā lomu piešķirē atbalsta vairākus galvenos un vairākus tvērumus. Tas atšķiras no *rbacApplication* resursu tipa. Microsoft Intune ir šāda RBAC pakalpojumu sniedzēja piemērs. Lomu piešķiršana intune var būt pamatsummu masīvs un tvērumu grupu masīvs. **Tas ir beta versijā, kas nozīmē, ka tas joprojām tiek izstrādāts un nav ieteicams lietošanai ražošanā.**
