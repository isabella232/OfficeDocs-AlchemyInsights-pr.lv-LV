---
title: Dynamics 365 veido uzņēmējdarbības noteikumiem - biznesa noteikumi netiek palaists formai
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 4ade8d2f68b465298e2d6efff3eef4f04f25c3bf
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/16/2019
ms.locfileid: "35748133"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>OnChange pasākums nenotiek programmiski mainot lauku

*OnChange* notikumu nerodas, ja lauks tiek mainīts programmatiski, izmantojot *atribūts.* [setValue](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) metodi. Ja vēlaties, lai notikumu apdarinātāji *OnChange* notikumu darboties pēc tam, kad jūs nosakiet vērtību, kas jāizmanto *formContext.data.entity atribūts.* [fireOnchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) metodes kodu.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
