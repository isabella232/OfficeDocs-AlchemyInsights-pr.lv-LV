---
title: Grupas izveide
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816363"
---
# <a name="create-a-group"></a><span data-ttu-id="7299c-102">Grupas izveide</span><span class="sxs-lookup"><span data-stu-id="7299c-102">Create a group</span></span>

<span data-ttu-id="7299c-103">Šajā tēmā ir aprakstīta grupu izveide.</span><span class="sxs-lookup"><span data-stu-id="7299c-103">This topic describes group creation.</span></span>

<span data-ttu-id="7299c-104">**Atļauja izveidot grupu**</span><span class="sxs-lookup"><span data-stu-id="7299c-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="7299c-105">Pārliecinieties, vai esat pilnvarots izveidot jaunu grupu.</span><span class="sxs-lookup"><span data-stu-id="7299c-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="7299c-106">Globālie administratori var atspējot grupu izveidi Azure portālā vai piekļuves panelī.</span><span class="sxs-lookup"><span data-stu-id="7299c-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="7299c-107">Iespējams, būs vajadzīgs administrators, lai izveidotu jaunu grupu jūsu vietā vai sniegtu jums atbilstošas atļaujas.</span><span class="sxs-lookup"><span data-stu-id="7299c-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="7299c-108">**Grupu izveides atļauju pārvaldība**</span><span class="sxs-lookup"><span data-stu-id="7299c-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="7299c-109">Globālie administratori var pārvaldīt grupu izveides atļaujas (ar drošību saistītu iemeslu dēļ) vai Office 365 grupas, kas izveidotas Azure portālā vai piekļuves panelī, izvēloties "Lietotāji var izveidot drošības grupas Azure portālā" vai "Lietotāji var izveidot Office 365 grupas Azure portālā" opcijas Sadaļā Vispārīgi  >  **(Iestatījumi).**</span><span class="sxs-lookup"><span data-stu-id="7299c-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="7299c-110">Varat arī ierobežot grupu izveidi, lai atlasītu lietotāju grupu, ja jums ir Azure Active Directory P1 Premium licence.</span><span class="sxs-lookup"><span data-stu-id="7299c-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="7299c-111">**Tiek atspējots paziņojums par esiet sveicināts! jauniem Office 365 grupas dalībniekiem**</span><span class="sxs-lookup"><span data-stu-id="7299c-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="7299c-112">Lietotājiem, kuri ir pievienoti Office 365 grupām, nosūtīto sveiciena paziņojumu var atspējot, Powershell iestatījumam **UnifiedGroupWelcomeMessageEnabled** iestatot vērtību False.</span><span class="sxs-lookup"><span data-stu-id="7299c-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="7299c-113">Uzziniet par šo iestatījumu [šeit.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="7299c-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

