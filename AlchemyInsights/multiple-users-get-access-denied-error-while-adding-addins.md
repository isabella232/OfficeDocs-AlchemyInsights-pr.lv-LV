---
title: Pievienojot pievienojumprogrammu programmā Outlook, vairāki lietotāji saņem piekļuves liegšanas kļūdu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424180"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="4baa3-102">Pievienojot pievienojumprogrammu programmā Outlook, vairāki lietotāji saņem piekļuves liegšanas kļūdu</span><span class="sxs-lookup"><span data-stu-id="4baa3-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="4baa3-103">Varat norādīt, kuriem jūsu organizācijas administratoriem ir atļaujas instalēt un pārvaldīt pievienojumprogrammas darbam ar Outlook.</span><span class="sxs-lookup"><span data-stu-id="4baa3-103">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook.</span></span> <span data-ttu-id="4baa3-104">Varat arī norādīt, kuriem lietotājiem jūsu organizācijā ir atļauja instalēt un pārvaldīt pievienojumprogrammas savām vajadzībām.</span><span class="sxs-lookup"><span data-stu-id="4baa3-104">You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="4baa3-105">Detalizētu informāciju skatiet rakstā [administratoru un lietotāju, kas var instalēt un pārvaldīt pievienojumprogrammas programmai Outlook, norādīšana](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="4baa3-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="4baa3-106">Lai pārliecinātos, vai esat veiksmīgi piešķīris lietotājam atļaujas, aizstājiet <Role Name> ar tās lomas nosaukumu, ko vēlaties pārbaudīt, un izpildiet šādu komandu pakalpojumā Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="4baa3-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="4baa3-107">Get-ManagementRoleAssignment-lomai " <Role Name> "-GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="4baa3-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="4baa3-108">Šajā piemērā ir parādīts, kā pārbaudīt, kam ir piešķirtas atļaujas, lai instalētu pievienojumprogrammas no Office veikala organizācijai.</span><span class="sxs-lookup"><span data-stu-id="4baa3-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="4baa3-109">PowerShell</span><span class="sxs-lookup"><span data-stu-id="4baa3-109">PowerShell</span></span>

<span data-ttu-id="4baa3-110">-Loma "organizācijas Marketplace lietojumprogrammas"-GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="4baa3-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="4baa3-111">Rezultātos Iegūstiet-ManagementRoleAssignment, pārskatiet ievadnes kolonnā efektīvie lietotāji.</span><span class="sxs-lookup"><span data-stu-id="4baa3-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="4baa3-112">Detalizētu informāciju par sintaksi un parametriem skatiet rakstā [iegūšana-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span><span class="sxs-lookup"><span data-stu-id="4baa3-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 