---
title: 902 (sinhronizācijas kļūdas, jo ir dublēti objekti)
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
ms.openlocfilehash: 33b8ad0a33eb02eb9ec5bd26f94b00e5645b3fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737348"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Sinhronizācijas kļūdas, ko rada objektu dublikāti

Veicot direktorija sinhronizēšanu programmā Microsoft 365, varat saņemt kādu no šiem kļūdas ziņojumiem:

- Nevar atjaunināt šo objektu Microsoft Online pakalpojumos, jo tālāk norādītajiem atribūtiem, kas saistīti ar šo objektu, ir vērtības, kas jau var būt saistītas ar citu objektu jūsu lokālajā direktorijā.

- Microsoft Online Services direktorijā jau pastāv sinhronizēts objekts ar tādu pašu starpniekservera adresi.

- Nevar atjaunināt šo objektu, jo tālāk norādītajiem atribūtiem, kas saistīti ar šo objektu, ir vērtības, kas jau var būt saistītas ar citu objektu lokālajā direktoriju pakalpojumos: UserPrincipalName.

Lai noteiktu un labotu problēmu, lejupielādējiet un palaidiet [IdFix DirSync kļūdu labošanas rīku](https://www.microsoft.com/download/details.aspx?id=36832).

Papildinformāciju skatiet rakstā [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
