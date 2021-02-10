---
title: Lietotāja piešķirtās pārvaldītās identitātes pārvaldība
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8211"
- "9003230"
ms.openlocfilehash: a44cb484b6d89e6d5f67b2900c38dde3610b0e23
ms.sourcegitcommit: 23e778f7414e5f1a98cc786146fe76d622b458bc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177582"
---
# <a name="manage-a-user-assigned-managed-identity"></a><span data-ttu-id="36c6c-102">Lietotāja piešķirtās pārvaldītās identitātes pārvaldība</span><span class="sxs-lookup"><span data-stu-id="36c6c-102">Manage a user-assigned managed identity</span></span>

<span data-ttu-id="36c6c-103">Lietotāja piešķirtās pārvaldītās identitātes pārvaldība ietver:</span><span class="sxs-lookup"><span data-stu-id="36c6c-103">The management of a user-assigned managed identity involves:</span></span>

- <span data-ttu-id="36c6c-104">Lomu piešķiršana lietotāja piešķirtai pārvaldītajai identitātei</span><span class="sxs-lookup"><span data-stu-id="36c6c-104">Assigning roles to a user-assigned managed identity</span></span>
- <span data-ttu-id="36c6c-105">Lietotāja piešķirtās pārvaldītās identitātes dzēšana</span><span class="sxs-lookup"><span data-stu-id="36c6c-105">Deleting a user-assigned managed identity</span></span>
- <span data-ttu-id="36c6c-106">Lietotāja piešķirtās pārvaldītās identitātes uzskaitīšana</span><span class="sxs-lookup"><span data-stu-id="36c6c-106">Listing a user-assigned managed identity</span></span>

<span data-ttu-id="36c6c-107">Papildinformāciju par iepriekš minētajiem uzdevumiem skatiet šajos rakstos:</span><span class="sxs-lookup"><span data-stu-id="36c6c-107">For more information on the tasks mentioned above, see the following articles:</span></span>

- <span data-ttu-id="36c6c-108">[Kā izveidot lietotāja piešķirtu pārvaldītu identitāti](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) — lomu piešķiršana lietotājam piešķirtai pārvaldītajai identitātei</span><span class="sxs-lookup"><span data-stu-id="36c6c-108">[How to create a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for assigning roles to a user-assigned managed identity</span></span>
- <span data-ttu-id="36c6c-109">[Kā izdzēst lietotāja piešķirtu pārvaldītu identitāti](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) — lietotāja piešķirtās pārvaldītās identitātes dzēšanai</span><span class="sxs-lookup"><span data-stu-id="36c6c-109">[How to delete a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for deleting a user-assigned managed identity</span></span>
- <span data-ttu-id="36c6c-110">[Kā uzskaitīt lietotāja piešķirtu pārvaldītu identitāti](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) — lietotāja piešķirtās pārvaldītās identitātes uzskaitīšana</span><span class="sxs-lookup"><span data-stu-id="36c6c-110">[How to list a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for listing a user-assigned managed identity</span></span>

> [!NOTE]
> <span data-ttu-id="36c6c-111">Pārbaudiet, vai jums ir **pārvaldītā identitātes līdzstrādnieka** lomas piešķiršana.</span><span class="sxs-lookup"><span data-stu-id="36c6c-111">Verify whether you have the **Managed Identity Contributor** role assignment.</span></span> <span data-ttu-id="36c6c-112">Šī lomas piešķiršana ir nepieciešama, lai izveidotu/dzēstu lietotāja piešķirtās pārvaldītās identitātes.</span><span class="sxs-lookup"><span data-stu-id="36c6c-112">That role assignment is required for creating/deleting user-assigned managed identities.</span></span>
