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
# <a name="rbac-rules"></a><span data-ttu-id="7f2b4-102">RBAC kārtulas</span><span class="sxs-lookup"><span data-stu-id="7f2b4-102">RBAC rules</span></span>

<span data-ttu-id="7f2b4-103">Ja saņemat atļauju kļūdu:</span><span class="sxs-lookup"><span data-stu-id="7f2b4-103">If you get the permission error:</span></span> 

- <span data-ttu-id="7f2b4-104">**Klientam ar objekta ID nav autorizācijas, lai veiktu darbības sfērā (kods: AuthorizationFailed)**: kad mēģināt izveidot resursu, pārbaudiet, vai pašlaik esat pierakstījies ar lietotāju, kuram ir piešķirta loma, kam atlasītajā tvērumā ir piešķirtas rakstīšanas atļaujas.</span><span class="sxs-lookup"><span data-stu-id="7f2b4-104">**The client with object id does not have authorization to perform action over scope (code: AuthorizationFailed)**: when you try to create a resource, check that you are currently signed in with a user that is assigned a role that has write permission to the resource at the selected scope.</span></span> <span data-ttu-id="7f2b4-105">Piemēram, lai pārvaldītu virtuālās mašīnas resursu grupā, jums ir jābūt [virtuālās mašīnas līdzstrādnieka](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) lomai resursu grupā (vai vecākobjekta tvērumā).</span><span class="sxs-lookup"><span data-stu-id="7f2b4-105">For example, to manage virtual machines in a resource group, you should have the [Virtual Machine Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) role on the resource group (or parent scope).</span></span> <span data-ttu-id="7f2b4-106">Katras iebūvētās lomas atļauju sarakstu skatiet rakstā [Azure resursu iebūvētās lomas](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="7f2b4-106">For a list of the permissions for each built-in role, see [Built-in roles for Azure resources](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="7f2b4-107">**Jums nav atļaujas izveidot atbalsta pieprasījumu**: kad mēģināt izveidot vai atjaunināt atbalsta biļeti, pārbaudiet, vai pašlaik esat pierakstījies ar lietotāju, kuram ir piešķirta loma ar Microsoft. support/supportTickets/Write atļauju, piemēram, [atbalsta pieprasījuma līdzstrādnieks](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span><span class="sxs-lookup"><span data-stu-id="7f2b4-107">**You don't have permission to create a support request**: when you try to create or update a support ticket, check that you are currently signed in with a user that is assigned a role that has the Microsoft.Support/supportTickets/write permission, such as [Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span></span>
- <span data-ttu-id="7f2b4-108">**Nevar izveidot papildu piešķirtās lomas (kods: RoleAssignmentLimitExceeded)**: kad mēģināt piešķirt lomu, mēģiniet samazināt lomu uzdevumu skaitu, to vietā piešķirot lomas grupām.</span><span class="sxs-lookup"><span data-stu-id="7f2b4-108">**No more role assignments can be created (code: RoleAssignmentLimitExceeded)**: when you try to assign a role, try to reduce the number of role assignments by assigning roles to groups instead.</span></span> <span data-ttu-id="7f2b4-109">Azure atbalsta līdz pat **2000** lomu uzdevumus katram abonementam.</span><span class="sxs-lookup"><span data-stu-id="7f2b4-109">Azure supports up to **2000** role assignments per subscription.</span></span>

<span data-ttu-id="7f2b4-110">Detalizētāku informāciju par Azure RBAC lomām skatiet sadaļā [AZURE RBAC lomas](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="7f2b4-110">For more details on Azure RBAC roles, see [Azure RBAC roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
