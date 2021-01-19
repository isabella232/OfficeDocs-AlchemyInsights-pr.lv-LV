---
title: Ar īpašnieku saistīto problēmu novēršana
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7815"
- "9004358"
ms.openlocfilehash: 914d5682a403197a8569bb75fda8a77449f485f6
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901002"
---
# <a name="troubleshoot-owner-issues"></a><span data-ttu-id="ba8ac-102">Ar īpašnieku saistīto problēmu novēršana</span><span class="sxs-lookup"><span data-stu-id="ba8ac-102">Troubleshoot owner issues</span></span>

<span data-ttu-id="ba8ac-103">Lai novērstu ar īpašnieku saistītās problēmas, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="ba8ac-103">To troubleshoot owner-related issues, perform the following steps:</span></span>

1. <span data-ttu-id="ba8ac-104">[Pievienojiet vai mainiet Azure abonementu administratorus](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): Azure Active Directory (Azure AD) grupas pieder un tās pārvalda grupas īpašnieki.</span><span class="sxs-lookup"><span data-stu-id="ba8ac-104">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): Azure Active Directory (Azure AD) groups are owned and managed by group owners.</span></span> <span data-ttu-id="ba8ac-105">Grupu īpašnieki var būt lietotāji vai pakalpojumu pamatprincipi, kā arī varat pārvaldīt grupu, tostarp dalību.</span><span class="sxs-lookup"><span data-stu-id="ba8ac-105">Group owners can be users or service principals, and are able to manage the group, including membership.</span></span> <span data-ttu-id="ba8ac-106">Grupas īpašniekus var piešķirt tikai esošie grupu īpašnieki vai grupu Administratori.</span><span class="sxs-lookup"><span data-stu-id="ba8ac-106">Only existing group owners or group-managing administrators can assign group owners.</span></span> <span data-ttu-id="ba8ac-107">Grupas īpašniekiem nav nepieciešami grupas dalībnieki.</span><span class="sxs-lookup"><span data-stu-id="ba8ac-107">Group owners aren't required to be members of the group.</span></span>
2. <span data-ttu-id="ba8ac-108">[Pievienojiet vai mainiet Azure abonementu administratorus](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator): šajā rakstā ir paskaidrots, kā pievienot vai mainīt administratora lomu lietotājam, kas izmanto Azure RBAC abonementu tvērumā.</span><span class="sxs-lookup"><span data-stu-id="ba8ac-108">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator): This article describes how to add or change the administrator role for a user using Azure RBAC at the subscription scope.</span></span>
3. <span data-ttu-id="ba8ac-109">Izmantojiet PowerShell, lai pievienotu grupas īpašnieku vai lietojumprogrammas īpašnieku.</span><span class="sxs-lookup"><span data-stu-id="ba8ac-109">Use PowerShell to add a group owner or an application owner.</span></span>
