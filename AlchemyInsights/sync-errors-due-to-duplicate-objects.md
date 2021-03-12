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
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708069"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Sinhronizācijas kļūdas, ko rada objektu dublikāti

Veicot direktorija sinhronizēšanu programmā Microsoft 365, varat saņemt kādu no šiem kļūdas ziņojumiem:

- Nevar atjaunināt šo objektu Microsoft Online pakalpojumos, jo tālāk norādītajiem atribūtiem, kas saistīti ar šo objektu, ir vērtības, kas jau var būt saistītas ar citu objektu jūsu lokālajā direktorijā.

- Microsoft Online Services direktorijā jau pastāv sinhronizēts objekts ar tādu pašu starpniekservera adresi.

- Nevar atjaunināt šo objektu, jo tālāk norādītajiem atribūtiem, kas saistīti ar šo objektu, ir vērtības, kas jau var būt saistītas ar citu objektu lokālajā direktoriju pakalpojumos: UserPrincipalName.

Lai noteiktu un labotu problēmu, lejupielādējiet un palaidiet [IdFix DirSync kļūdu labošanas rīku](https://github.com/Microsoft/idfix).

Papildinformāciju skatiet rakstā [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
