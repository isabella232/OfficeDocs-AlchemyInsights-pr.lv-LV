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
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="eea3f-102">Sinhronizācijas kļūdas, ko rada objektu dublikāti</span><span class="sxs-lookup"><span data-stu-id="eea3f-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="eea3f-103">Veicot direktorija sinhronizēšanu programmā Microsoft 365, varat saņemt kādu no šiem kļūdas ziņojumiem:</span><span class="sxs-lookup"><span data-stu-id="eea3f-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="eea3f-104">Nevar atjaunināt šo objektu Microsoft Online pakalpojumos, jo tālāk norādītajiem atribūtiem, kas saistīti ar šo objektu, ir vērtības, kas jau var būt saistītas ar citu objektu jūsu lokālajā direktorijā.</span><span class="sxs-lookup"><span data-stu-id="eea3f-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="eea3f-105">Microsoft Online Services direktorijā jau pastāv sinhronizēts objekts ar tādu pašu starpniekservera adresi.</span><span class="sxs-lookup"><span data-stu-id="eea3f-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="eea3f-106">Nevar atjaunināt šo objektu, jo tālāk norādītajiem atribūtiem, kas saistīti ar šo objektu, ir vērtības, kas jau var būt saistītas ar citu objektu lokālajā direktoriju pakalpojumos: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="eea3f-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="eea3f-107">Lai noteiktu un labotu problēmu, lejupielādējiet un palaidiet [IdFix DirSync kļūdu labošanas rīku](https://github.com/Microsoft/idfix).</span><span class="sxs-lookup"><span data-stu-id="eea3f-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://github.com/Microsoft/idfix).</span></span>

<span data-ttu-id="eea3f-108">Papildinformāciju skatiet rakstā [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="eea3f-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
