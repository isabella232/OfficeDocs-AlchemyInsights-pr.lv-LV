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
# <a name="hide-public-folders"></a>Publisko mapju paslēpšana

**Lai paslēptu visu publisko mapju koku**:

Izmantojiet [šajā](https://aka.ms/ControlPF) rakstā norādītās darbības, lai paslēptu visu publisko mapju koku no selektīvajiem vai visiem lietotājiem.

**Lai paslēptu konkrētu publisko mapi**:

1. Atļauju pievienošana lietotājiem, kuriem ir jāpiekļūst publiskajai mapei

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. Noņemiet lietotāja **noklusējumu** no **atļauju** saraksta:

    `Remove-PublicFolderClientPermission \test1 -User Default`
