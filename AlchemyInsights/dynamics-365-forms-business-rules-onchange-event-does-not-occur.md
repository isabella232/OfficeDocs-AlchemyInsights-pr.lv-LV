---
title: Dynamics 365 Forms biznesa kārtulas-biznesa kārtulu Nededzinot veidlapas
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: cbdedd2c5fcf5517243e60e36d86479d6c3f7814
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/25/2019
ms.locfileid: "36529026"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Notikumu OnChange nerodas, ja lauks tiek mainīts programmiski

Notikumu *onchange* nerodas, ja lauks tiek mainīts programmiski, izmantojot *atribūtu.* [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) metodi. Ja nepieciešams notikumu apdarinātāji *onchange* notikumu palaist pēc vērtību, jāizmanto *formcontext. Data. ENTITY atribūts.* [Fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) metodi savā kodā.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
