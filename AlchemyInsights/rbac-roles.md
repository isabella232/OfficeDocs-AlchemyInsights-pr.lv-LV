---
title: 'RBAC lomas '
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
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583549"
---
# <a name="rbac-rules"></a>RBAC kārtulas

Ja saņemat atļauju kļūdu: 

- **Klientam ar objekta ID nav autorizācijas, lai veiktu darbības sfērā (kods: AuthorizationFailed)**: kad mēģināt izveidot resursu, pārbaudiet, vai pašlaik esat pierakstījies ar lietotāju, kuram ir piešķirta loma, kam atlasītajā tvērumā ir piešķirtas rakstīšanas atļaujas. Piemēram, lai pārvaldītu virtuālās mašīnas resursu grupā, jums ir jābūt [virtuālās mašīnas līdzstrādnieka](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) lomai resursu grupā (vai vecākobjekta tvērumā). Katras iebūvētās lomas atļauju sarakstu skatiet rakstā [Azure resursu iebūvētās lomas](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).
- **Jums nav atļaujas izveidot atbalsta pieprasījumu**: kad mēģināt izveidot vai atjaunināt atbalsta biļeti, pārbaudiet, vai pašlaik esat pierakstījies ar lietotāju, kuram ir piešķirta loma ar Microsoft. support/supportTickets/Write atļauju, piemēram, [atbalsta pieprasījuma līdzstrādnieks](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).
- **Nevar izveidot papildu piešķirtās lomas (kods: RoleAssignmentLimitExceeded)**: kad mēģināt piešķirt lomu, mēģiniet samazināt lomu uzdevumu skaitu, to vietā piešķirot lomas grupām. Azure atbalsta līdz pat **2000** lomu uzdevumus katram abonementam.

Detalizētāku informāciju par Azure RBAC lomām skatiet sadaļā [AZURE RBAC lomas](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
