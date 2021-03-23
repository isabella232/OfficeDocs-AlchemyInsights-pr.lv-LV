---
title: Microsoft Edge modificēšana, izmantojot datu direktorija mainīgos, nevis nešifrētos ceļus
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8222"
- "9004596"
ms.openlocfilehash: 23ce69157c465c56d0fc5ada7c2c159e3192fd75
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035821"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a>Microsoft Edge modificēšana, izmantojot datu direktorija mainīgos, nevis nešifrētos ceļus

Piemēram, operētājsistēmā Windows, lai glabātu profila datus lietotāja lokālās lietojumprogrammas datos, nevis noklusējuma atrašanās vietā, iestatiet *UserDataDir* politiku uz **$ {local_app_data} \Edge\Profile**.

Lai iegūtu papildinformāciju, skatiet rakstu [Microsoft Edge lietotāju datu direktorija mainīgo izveide](https://docs.microsoft.com/deployedge/microsoft-edge-policies).