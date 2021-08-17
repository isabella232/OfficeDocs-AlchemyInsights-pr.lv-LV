---
title: ExO publiskā mape Ar iespējotu pastu sūtīšana
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: 22aa3e8f46c2ff4f62cb520b9498041dffb9d3a3eb607d788cc97b10bf32dbb5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052573"
---
# <a name="sendas-mail-enabled-public-folder"></a>Publiska mape Sūtīt kā pastu, kurā iespējots

Šajā piemērā lietotājam Jason tiek piešķirtas atļaujas "Nosūtīt kā" publiskai mapei NewPF1, kurā iespējots pasts.

Add-RecipientPermission -Identity 'NewPF1' -Trustee "Jason" -AccessRights 'SendAs'

Detalizētu informāciju par sintaksi un parametriem skatiet rakstā Atļauju nosūtīt kā vai Nosūtīt kā vārdā piešķiršana publiskajām mapēm ar [iespējotu pastu.](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs)

