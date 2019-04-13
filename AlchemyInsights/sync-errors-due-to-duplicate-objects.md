---
title: 902 (sinhronizācijas kļūdas dēļ objektu dublikātus)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: ce7eeb07cfde16e6d6856a9369c042dcf4f05b63
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/13/2019
ms.locfileid: "31859111"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Sinhronizācijas kļūdas dēļ objektu dublikātus

Varat saņemt kādu no šiem kļūdas ziņojumiem pēc direktoriju sinhronizācijas pabeigšanas:

- Nevar atjaunināt šo objektu Microsoft tiešsaistes pakalpojumus, jo šādi atribūti, kas saistīti ar šo objektu ir vērtības, kas jau var būt saistīta ar citu objektu jūsu lokālajā direktorijā.

- Sinhronizēto objekts ar tādu pašu starpniekservera adresi Microsoft tiešsaistes pakalpojumu direktorijs jau pastāv.

- Nevar atjaunināt šajā objektā, jo šādi atribūti, kas saistīti ar šo objektu ir vērtības, kas jau var būt saistīta ar citu objektu lokālo direktoriju pakalpojumos: UserPrincipalName.

Lai identificētu un labotu problēmu, lejupielādēt un palaist [IdFix DirSync kļūdu labošanas rīks](https://www.microsoft.com/download/details.aspx?id=36832).

Plašāku informāciju skatiet [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
