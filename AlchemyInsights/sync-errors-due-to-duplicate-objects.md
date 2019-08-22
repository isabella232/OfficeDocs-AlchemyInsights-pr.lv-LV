---
title: 902 (sinhronizācijas kļūdas dēļ objektu dublikātus)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 777c2d8d530d03d58180f43b362ee065439b56b3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507422"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Sinhronizācijas kļūdas dēļ objektu dublikātus

Jūs varētu saņemt kādu no šiem kļūdas ziņojumiem, kad directory sinhronizācija ir pabeidzis Office 365:

- Nevar atjaunināt šo objektu Microsoft tiešsaistes pakalpojumus, jo šādi atribūti, kas saistīti ar šo objektu ir vērtības, kas jau var būt saistīta ar citu objektu jūsu lokālajā direktorijā.

- Sinhronizēto objekts ar tādu pašu starpniekservera adresi Microsoft tiešsaistes pakalpojumu direktorijs jau pastāv.

- Nevar atjaunināt šajā objektā, jo šādi atribūti, kas saistīti ar šo objektu ir vērtības, kas jau var būt saistīta ar citu objektu lokālo direktoriju pakalpojumos: UserPrincipalName.

Lai identificētu un labotu problēmu, lejupielādēt un palaist [IdFix DirSync kļūdu labošanas rīks](https://www.microsoft.com/download/details.aspx?id=36832).

Plašāku informāciju skatiet [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
