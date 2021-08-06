---
title: 'Lomu lomu '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 1faa9f69942d39b8d78c8f3e1316f93b52eeede6408dfabc89d0f7fe38b86fb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923138"
---
# <a name="rbac-rules"></a>RBAC kārtulas

Ja tiek parādīts atļaujas kļūdas ziņojums: 

- Klientam ar objekta ID nav autorizācijas veikt darbības ar tvērumu **(kods: AuthorizationFailed):** mēģinot izveidot resursu, pārbaudiet, vai pašlaik esat pierakstījies ar lietotāju, kuram ir piešķirta loma, kam ir rakstīšanas atļauja resursam atlasītajā tvērumā. Piemēram, lai pārvaldītu virtuālās mašīnas resursu grupā, [](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) jums jābūt virtuālās mašīnas līdzstrādnieka lomai resursu grupā (vai vecākobjekta tvērumā). Katras iebūvētās lomas atļauju sarakstu skatiet rakstā [Iebūvētās lomas Azure resursiem.](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)
- Jums nav atļaujas izveidot atbalsta **pieprasījumu:** kad mēģināt izveidot vai atjaunināt atbalsta biļeti, pārbaudiet, vai pašlaik esat pierakstījies ar lietotāju, kuram ir piešķirta loma Ar Microsoft.Support/supportTickets/write atļauju, piemēram, atbalsta pieprasījumu līdzstrādnieks. [](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)
- Vairs nevar izveidot lomu piešķiri **(kods: RoleAssignmentLimitExceeded):** mēģinot piešķirt lomu, mēģiniet samazināt lomu piešķires skaitu, tā vietā piešķirot lomas grupām. Azure atbalsta līdz **pat 2000 lomu** piešķires katram abonementam.

Papildinformāciju par Azure RBAC lomām skatiet rakstā [Azure RBAC lomas.](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support)
