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
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="f8bd6-102">Notikumu OnChange nerodas, ja lauks tiek mainīts programmiski</span><span class="sxs-lookup"><span data-stu-id="f8bd6-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="f8bd6-103">Notikumu *onchange* nerodas, ja lauks tiek mainīts programmiski, izmantojot *atribūtu.* [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) metodi.</span><span class="sxs-lookup"><span data-stu-id="f8bd6-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="f8bd6-104">Ja nepieciešams notikumu apdarinātāji *onchange* notikumu palaist pēc vērtību, jāizmanto *formcontext. Data. ENTITY atribūts.* [Fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) metodi savā kodā.</span><span class="sxs-lookup"><span data-stu-id="f8bd6-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute.*[fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
