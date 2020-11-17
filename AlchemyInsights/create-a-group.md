---
title: Grupas izveide
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088907"
---
# <a name="create-a-group"></a><span data-ttu-id="92e71-102">Grupas izveide</span><span class="sxs-lookup"><span data-stu-id="92e71-102">Create a group</span></span>

<span data-ttu-id="92e71-103">Šajā tēmā ir aprakstīta grupas izveide.</span><span class="sxs-lookup"><span data-stu-id="92e71-103">This topic describes group creation.</span></span>

<span data-ttu-id="92e71-104">**Atļauja izveidot grupu**</span><span class="sxs-lookup"><span data-stu-id="92e71-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="92e71-105">Pārliecinieties, vai jums ir atļauja izveidot jaunu grupu.</span><span class="sxs-lookup"><span data-stu-id="92e71-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="92e71-106">Globālie administratori var atspējot grupu izveidi Azure portālā vai piekļuves panelī.</span><span class="sxs-lookup"><span data-stu-id="92e71-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="92e71-107">Iespējams, ka jums ir nepieciešams administrators, lai izveidotu jaunu grupu vai piešķirtu atbilstošas atļaujas.</span><span class="sxs-lookup"><span data-stu-id="92e71-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="92e71-108">**Grupu izveides atļauju pārvaldība**</span><span class="sxs-lookup"><span data-stu-id="92e71-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="92e71-109">Globālie administratori var pārvaldīt grupu izveides atļaujas (ar drošību saistītus iemeslus) vai Office 365 grupas, kas izveidotas Azure portālā vai piekļuves panelī, izvēloties "lietotāji var izveidot drošības grupas Azure portāliem" vai "lietotāji var izveidot Office 365 grupas Azure portāli" opcijas visās **grupās**  >  **Vispārīgi (iestatījumi)**.</span><span class="sxs-lookup"><span data-stu-id="92e71-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="92e71-110">Varat arī ierobežot grupu izveidi, lai atlasītu lietotāju grupu, ja jums ir Azure Active Directory P1 Premium licence.</span><span class="sxs-lookup"><span data-stu-id="92e71-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="92e71-111">**Sveiciena paziņojuma par jauniem Office 365 grupas dalībniekiem atspējošana**</span><span class="sxs-lookup"><span data-stu-id="92e71-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="92e71-112">Sveiciena paziņojumu, kas nosūtīts lietotājiem, kuri tiek pievienoti Office 365 grupām, var atspējot, iestatot **UnifiedGroupWelcomeMessageEnabled** uz Aplams programmā PowerShell.</span><span class="sxs-lookup"><span data-stu-id="92e71-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="92e71-113">Uzziniet par šo iestatījumu [šeit](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="92e71-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

