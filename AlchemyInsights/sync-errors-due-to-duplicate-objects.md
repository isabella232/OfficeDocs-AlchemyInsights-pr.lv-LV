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
ms.openlocfilehash: 06cd582c30a59a94ee117728bd5daebecca77bc8
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758002"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="fcb85-102">Sinhronizācijas kļūdas dēļ objektu dublikātus</span><span class="sxs-lookup"><span data-stu-id="fcb85-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="fcb85-103">Varat saņemt kādu no šiem kļūdas ziņojumiem pēc direktoriju sinhronizācijas pabeigšanas:</span><span class="sxs-lookup"><span data-stu-id="fcb85-103">You might receive one of the following error messages when directory synchronization finishes:</span></span>

- <span data-ttu-id="fcb85-104">Nevar atjaunināt šo objektu Microsoft tiešsaistes pakalpojumus, jo šādi atribūti, kas saistīti ar šo objektu ir vērtības, kas jau var būt saistīta ar citu objektu jūsu lokālajā direktorijā.</span><span class="sxs-lookup"><span data-stu-id="fcb85-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="fcb85-105">Sinhronizēto objekts ar tādu pašu starpniekservera adresi Microsoft tiešsaistes pakalpojumu direktorijs jau pastāv.</span><span class="sxs-lookup"><span data-stu-id="fcb85-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="fcb85-106">Nevar atjaunināt šajā objektā, jo šādi atribūti, kas saistīti ar šo objektu ir vērtības, kas jau var būt saistīta ar citu objektu lokālo direktoriju pakalpojumos: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="fcb85-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="fcb85-107">Lai identificētu un labotu problēmu, lejupielādēt un palaist [IdFix DirSync kļūdu labošanas rīks](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="fcb85-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="fcb85-108">Plašāku informāciju skatiet [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="fcb85-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
