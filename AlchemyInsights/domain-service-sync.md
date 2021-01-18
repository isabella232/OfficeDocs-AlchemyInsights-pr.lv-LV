---
title: Domēna pakalpojuma sinhronizācija
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.openlocfilehash: b35d3a402bc08a27a818209385c5666b901fa524
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885153"
---
# <a name="domain-service-synchronization"></a><span data-ttu-id="46260-102">Domēna pakalpojuma sinhronizācija</span><span class="sxs-lookup"><span data-stu-id="46260-102">Domain service synchronization</span></span>

<span data-ttu-id="46260-103">Objekti un akreditācijas dati Azure Active Directory domēna pakalpojumos (Azure AD DS) pārvaldītā domēnā var izveidot lokāli vai sinhronizēti no Azure Active Directory (Azure AD) nomnieka.</span><span class="sxs-lookup"><span data-stu-id="46260-103">Objects and credentials in an Azure Active Directory Domain Services (Azure AD DS) managed domain can either be created locally within the domain, or synchronized from an Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="46260-104">Pirmoreiz izvietojot Azure AD DS, automātiskā vienvirziena sinhronizācija ir konfigurēta un uzsākta, lai replicētu objektus no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="46260-104">When you first deploy Azure AD DS, an automatic one-way synchronization is configured and initiated to replicate the objects from Azure AD.</span></span> <span data-ttu-id="46260-105">Šī vienvirziena sinhronizācija turpina darboties fonā, lai nodrošinātu Azure AD DS pārvaldītā domēna atjaunināšanu ar jebkādām izmaiņām Azure AD.</span><span class="sxs-lookup"><span data-stu-id="46260-105">This one-way synchronization continues to run in the background to keep the Azure AD DS managed domain up-to-date with any changes from Azure AD.</span></span> <span data-ttu-id="46260-106">Azure AD DS atgriežoties Azure AD, sinhronizācija netiek veikta.</span><span class="sxs-lookup"><span data-stu-id="46260-106">No synchronization occurs from Azure AD DS back to Azure AD.</span></span>

<span data-ttu-id="46260-107">Detalizētu informāciju par Azure Active Directory domēna pakalpojumu sinhronizāciju skatiet sadaļā [Domain Service sinhronizācija](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span><span class="sxs-lookup"><span data-stu-id="46260-107">For more details on Azure Active Directory domain service synchronization, see [Domain Service Synchronization](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span></span> 
