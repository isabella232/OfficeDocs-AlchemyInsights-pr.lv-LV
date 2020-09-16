---
title: Par identitāti pakalpojumā Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664177"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="f66d8-102">Par identitāti pakalpojumā Yammer</span><span class="sxs-lookup"><span data-stu-id="f66d8-102">About identity in Yammer</span></span>

<span data-ttu-id="f66d8-103">Ieteicams visiem tīkliem veikt tālāk norādītās darbības, lai novērstu ar identitāti saistītas problēmas:</span><span class="sxs-lookup"><span data-stu-id="f66d8-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="f66d8-104">Uzspiest Office 365 identitāti pēc Microsoft 365 kontu nodrošināšanas lietotājiem Azure AD, lai nodrošinātu, ka visi lietotāji pierakstās, izmantojot savu galveno Microsoft 365 kontu.</span><span class="sxs-lookup"><span data-stu-id="f66d8-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="f66d8-105">Papildinformāciju skatiet rakstā [Office 365 identitātes ieviešana Yammer lietotājiem](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span><span class="sxs-lookup"><span data-stu-id="f66d8-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="f66d8-106">Apvienot vairākus Yammer tīklus.</span><span class="sxs-lookup"><span data-stu-id="f66d8-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="f66d8-107">Mantotās Yammer konfigurācijas atļauj vairākiem Yammer tīkliem izveidot savienojumu ar vienu nomnieku.</span><span class="sxs-lookup"><span data-stu-id="f66d8-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="f66d8-108">Papildinformāciju skatiet rakstā [tīkla migrācija: vairāku Yammer tīklu konsolidēšana](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="f66d8-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="f66d8-109">Ja vēlaties, varat ieviest Yammer licencēšanu, lai bloķētu Yammer lietotājus, ja viņiem nav licences.</span><span class="sxs-lookup"><span data-stu-id="f66d8-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="f66d8-110">Papildinformāciju skatiet rakstā [Yammer lietotāju licenču pārvaldība pakalpojumā Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="f66d8-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="f66d8-111">Visbeidzot, audits lietotāju saraksts vecākiem Yammer tīkliem un aizturēt mantotos lietotājus.</span><span class="sxs-lookup"><span data-stu-id="f66d8-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="f66d8-112">Ieteicams aizturēt (deaktivizēt) lietotājus, nevis izdzēst tos, jo dzēšana ir neatgriezeniska.</span><span class="sxs-lookup"><span data-stu-id="f66d8-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="f66d8-113">Papildinformāciju skatiet rakstā [Yammer lietotāju auditi tīklos, kas saistīti ar Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) , un [Lietotāju noņemšana](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span><span class="sxs-lookup"><span data-stu-id="f66d8-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="f66d8-114">Konfigurējot Yammer, veicot tālāk norādītās darbības, jūs varēsit arī konfigurēt savu Yammer tīklu Microsoft 365 vietējais režīms.</span><span class="sxs-lookup"><span data-stu-id="f66d8-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="f66d8-115">Papildinformāciju skatiet rakstā [Yammer tīkla konfigurēšana Microsoft 365 vietējā režīmā](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span><span class="sxs-lookup"><span data-stu-id="f66d8-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>