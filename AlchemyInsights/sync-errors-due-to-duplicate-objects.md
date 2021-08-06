---
title: 902 (Sinhronizācijas kļūdas objektu dublikātu dēļ)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: a047afd63484423520ed80fbf223f0e50f3e02624bd9859d4dcbbd94cf23143f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998801"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Sinhronizēt kļūdas objektu dublikātu dēļ

Kad direktorija sinhronizēšana tiek pabeigta produktā, iespējams, tiks parādīts Microsoft 365:

- Nevar atjaunināt šo objektu pakalpojumā Microsoft Online Services, jo tālāk sniegtajiem atribūtiem, kas saistīti ar šo objektu, ir vērtības, kas, iespējams, jau ir saistītas ar citu objektu jūsu lokālajā direktorijā.

- Sinhronizēts objekts ar to pašu starpniekservera adresi jau pastāv jūsu Microsoft Online Services direktorijā.

- Nevar atjaunināt šo objektu, jo šiem atribūtiem, kas saistīti ar šo objektu, ir vērtības, kas, iespējams, jau ir saistītas ar citu objektu jūsu lokālā direktorija pakalpojumos: UserPrincipalName.

Lai noteiktu un novērstu šo problēmu, lejupielādējiet un palaidiet [IdFix DirSync kļūdu labošanas rīku.](https://github.com/Microsoft/idfix)

Papildinformāciju skatiet [rakstā KB2647098.](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)
