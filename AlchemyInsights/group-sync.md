---
title: Grupas sinhronizācija
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8304"
- "9003234"
ms.openlocfilehash: 52c19b6dcc79968150a188b389c5481c122f7945
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256793"
---
# <a name="group-sync"></a><span data-ttu-id="8b755-102">Grupas sinhronizācija</span><span class="sxs-lookup"><span data-stu-id="8b755-102">Group sync</span></span>

<span data-ttu-id="8b755-103">Šajā rakstā ir sniegta informācija par grupas sinhronizēšanu.</span><span class="sxs-lookup"><span data-stu-id="8b755-103">This article provides guidance on group synchronization.</span></span>

1. <span data-ttu-id="8b755-104">Ja globālais administrators vai grupas īpašnieks nevar modificēt grupas rekvizītus vai pievienot dalībniekus vai piešķirt īpašniekus Azure portālā, pārliecinieties, vai šīs grupas iestādes avots ir Azure Active Directory (Azure AD) globālā administratora vai grupas īpašniekam, lai modificētu grupu.</span><span class="sxs-lookup"><span data-stu-id="8b755-104">If a global admin or group owner is not able to modify group properties or add members or assign owners in the Azure portal, ensure the source of the authority for the group is Azure Active Directory (Azure AD) for the global admin or group owner to modify the group.</span></span>
2. <span data-ttu-id="8b755-105">Pirms mēģināt dzēst sinhronizētu grupu Azure AD, pārliecinieties, vai esat [izdzēsis visas piešķirtās licences](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) , lai novērstu kļūdas.</span><span class="sxs-lookup"><span data-stu-id="8b755-105">Before attempting to delete a synced group in Azure AD, ensure you have [deleted all assigned licenses](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) to avoid errors.</span></span>

<span data-ttu-id="8b755-106">Lai iegūtu informāciju par to, kā sinhronizēt lietotājus, grupas un kontaktpersonas, skatiet rakstu [AZURE ad Connect sinhronizācija](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts)un izpildiet [lokālās grupas sinhronizēšanu Azure, izmantojot Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) , lai sinhronizētu, izmantojot ad Connect.</span><span class="sxs-lookup"><span data-stu-id="8b755-106">For understanding how to sync users, groups and contacts, see [Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts), and follow [Syncing an on-premises group to Azure using Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) to sync on-perm groups using AD connect.</span></span>

<span data-ttu-id="8b755-107">Izmantojiet šo rokasgrāmatu, lai novērstu kļūdas, kas rodas [sinhronizācijas laikā](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) , lai novērstu bieži sastopamas kļūdas sinhronizācijas laikā.</span><span class="sxs-lookup"><span data-stu-id="8b755-107">Follow this guide [Troubleshooting Errors during synchronization](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) to troubleshoot common errors during synchronization.</span></span>

