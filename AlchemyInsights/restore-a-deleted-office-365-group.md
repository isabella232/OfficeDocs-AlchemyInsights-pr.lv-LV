---
title: Izdzēstas Microsoft 365 grupas atjaunošana
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: caa2c8987eecb89bac3469bf9471847858cab0ba
ms.sourcegitcommit: ec99a3a2e1e6a13d9a829d65ad1692a607dc3a17
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/06/2021
ms.locfileid: "51597450"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="5b7f5-102">Izdzēstas Microsoft 365 grupas atjaunošana</span><span class="sxs-lookup"><span data-stu-id="5b7f5-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="5b7f5-103">Izdzēstu Microsoft 365 grupu vai Microsoft Teams varat atjaunot 30 dienu laikā pēc dzēšanas.</span><span class="sxs-lookup"><span data-stu-id="5b7f5-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="5b7f5-104">Dodieties uz [Microsoft 365 administrēšanas centru,](https://aka.ms/RestoreDeletedGroup) lai pieteiktos un uzskaitītu izdzēstās grupas un grupas.</span><span class="sxs-lookup"><span data-stu-id="5b7f5-104">Go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup) to log in and list the deleted groups and teams.</span></span>

    <span data-ttu-id="5b7f5-105">**Piezīme.** Piesakieties, izmantojot kontu, kas ir piešķirts nomnieka administratoram vai grupu administratora lomai.</span><span class="sxs-lookup"><span data-stu-id="5b7f5-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="5b7f5-106">Atlasiet izdzēsto Microsoft 365 grupu/grupu, kas jāatjauno, un noklikšķiniet **uz Atjaunot grupu**.</span><span class="sxs-lookup"><span data-stu-id="5b7f5-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="5b7f5-107">Ja grupu nevar atjaunot konfliktējošas SMTP adreses dēļ, izmantojiet tālāk norādīto komandu, lai atrastu objektu, kas izraisa konfliktu, un noņemtu SMTP adresi:</span><span class="sxs-lookup"><span data-stu-id="5b7f5-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="5b7f5-108">**Piezīme.** Dažos gadījumos grupas un visu tās datu atjaunošana var ilgt līdz pat 24 stundām.</span><span class="sxs-lookup"><span data-stu-id="5b7f5-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="5b7f5-109">Lai iegūtu papildinformāciju vai uzzinātu, kā atjaunot grupas, izmantojot PowerShell, skatiet rakstu [Izdzēstas Microsoft 365 grupas atjaunošana.](https://go.microsoft.com/fwlink/?linkid=867802)</span><span class="sxs-lookup"><span data-stu-id="5b7f5-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>