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
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="bde8f-102">OnChange pasākums nenotiek programmiski mainot lauku</span><span class="sxs-lookup"><span data-stu-id="bde8f-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="bde8f-103">*OnChange* notikumu nerodas, ja lauks tiek mainīts programmatiski, izmantojot *atribūts.* [setValue](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) metodi.</span><span class="sxs-lookup"><span data-stu-id="bde8f-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="bde8f-104">Ja vēlaties, lai notikumu apdarinātāji *OnChange* notikumu darboties pēc tam, kad jūs nosakiet vērtību, kas jāizmanto *formContext.data.entity atribūts.* [fireOnchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) metodes kodu.</span><span class="sxs-lookup"><span data-stu-id="bde8f-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute.*[fireOnchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
