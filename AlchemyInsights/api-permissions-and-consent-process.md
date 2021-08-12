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
ms.openlocfilehash: 078f5798533dfbbf97858f305729f103663644fee3590cdcc877233041adae81
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932068"
---
# <a name="api-permissions-and-consent-process"></a>API atļaujas un piekrišanas process

Lai jūsu programma varētu piekļūt Microsoft Graph datiem, lietotājam vai administratoram tā ir jāpiešķir pareizās atļaujas, izmantojot piekrišanas procesu. [Microsoft Graph atsaucē ir](https://docs.microsoft.com/graph/permissions-reference) uzskaitītas atļaujas, kas saistītas ar katru galveno Microsoft Graph API kopu. Tajā arī sniegti norādījumi par atļauju lietošanu.

**Pakalpojuma pamatsummas iestatīšana vai atjaunināšana**

- [Create serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) — šajā rakstā paskaidrots, kā izveidot jaunu servicePrincipal objektu.
- [Azure AD lietojumprogrammas &](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) pamatnosauka izveide portālā — šajā rakstā ir parādīts, kā izveidot jaunu Azure Active Directory (Azure AD) lietojumprogrammu un pakalpojuma galveno nosaukumu, ko var izmantot ar lomu piekļuves vadību.
- [Lietojumprogrammas &](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) pakalpojuma pamatnosaucību pakalpojumā Azure AD — šajā rakstā aprakstīta lietojumprogrammu reģistrācija, lietojumprogrammu objekti un pakalpojuma pamatsumma pakalpojumā Azure Active Directory: kas tās ir, kā tās tiek izmantotas un kā tās ir saistītas savā starpā.

**Pievienot vai atjaunināt lietojumprogrammu reģistrāciju un sniegt administratora piekrišanu**

- [Lietojumprogrammas reģistrācijas](https://docs.microsoft.com/graph/api/application-post-applications) izveide — šajā rakstā paskaidrots, kā izveidot jaunu lietojumprogrammas objektu.
- [Atjaunināt lietojumprogrammas reģistrāciju — API](https://docs.microsoft.com/graph/api/application-update) atļaujas — šajā rakstā aprakstīts, kā atjaunināt lietojumprogrammas objekta rekvizītus.
- [Sniedziet administratora piekrišanu](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) — administratora piekrišanai un vispār piekrišanai mēs pieprasām, lai administrators sniegtu atļauju tieši.
- [RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) — lomu pārvaldības konteiners vienotām lomu definīcijām un lomu piešķirēm Microsoft 365 RBAC pakalpojumu sniedzējiem, kas vienā lomu piešķirē atbalsta vairākus galvenos un vairākus tvērumus. Tas atšķiras no *rbacApplication* resursu tipa. Microsoft Intune ir šāda RBAC nodrošinātāja piemērs. Lomu piešķiršana intune var būt pamatsummu masīvs un tvērumu grupu masīvs. **Tas ir beta versijā, kas nozīmē, ka tas joprojām tiek izstrādāts un nav ieteicams lietošanai ražošanā.**
