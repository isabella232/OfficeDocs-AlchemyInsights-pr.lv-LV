---
title: Publisko mapju paslēpšana
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/18/2021
ms.locfileid: "50315374"
---
# <a name="hide-public-folders"></a><span data-ttu-id="3514c-102">Publisko mapju paslēpšana</span><span class="sxs-lookup"><span data-stu-id="3514c-102">Hide public folders</span></span>

<span data-ttu-id="3514c-103">**Lai paslēptu visu publisko mapju koku**:</span><span class="sxs-lookup"><span data-stu-id="3514c-103">**To hide entire public folder tree**:</span></span>

<span data-ttu-id="3514c-104">Izmantojiet [šajā](https://aka.ms/ControlPF) rakstā norādītās darbības, lai paslēptu visu publisko mapju koku no selektīvajiem vai visiem lietotājiem.</span><span class="sxs-lookup"><span data-stu-id="3514c-104">Use the steps in [this](https://aka.ms/ControlPF) article to hide entire public folder tree from selective or all users.</span></span>

<span data-ttu-id="3514c-105">**Lai paslēptu konkrētu publisko mapi**:</span><span class="sxs-lookup"><span data-stu-id="3514c-105">**To hide a specific public folder**:</span></span>

1. <span data-ttu-id="3514c-106">Atļauju pievienošana lietotājiem, kuriem ir jāpiekļūst publiskajai mapei</span><span class="sxs-lookup"><span data-stu-id="3514c-106">Add permissions for users who need to access the public folder</span></span>

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. <span data-ttu-id="3514c-107">Noņemiet lietotāja **noklusējumu** no **atļauju** saraksta:</span><span class="sxs-lookup"><span data-stu-id="3514c-107">Remove the user **Default** from the **permission** list:</span></span>

    `Remove-PublicFolderClientPermission \test1 -User Default`
