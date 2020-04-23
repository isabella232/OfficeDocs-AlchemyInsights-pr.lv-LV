---
title: Profila sinhronizācija
ms.author: arnek
author: arnek
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: dc6e0280961d14aa3e6bd466afbe0cbe89418d17
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43768120"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="931dd-102">Kad mana profila izmaiņas sinhronizācija ar SharePoint lietotāja profila lietojumprogrammu?</span><span class="sxs-lookup"><span data-stu-id="931dd-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="931dd-103">SharePoint Online izmanto Active Directory importēšanas taimera darbu (AD Import) importēt lietotāju un grupu lietotāja profila lietojumprogrammā.</span><span class="sxs-lookup"><span data-stu-id="931dd-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="931dd-104">REKLĀMAS importēšana sinhronizē izmaiņas no SharePoint Online Directory krātuves lietotāja profila lietojumprogrammu.</span><span class="sxs-lookup"><span data-stu-id="931dd-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="931dd-105">Šīs izmaiņas tiek apstrādātas partijās.</span><span class="sxs-lookup"><span data-stu-id="931dd-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="931dd-106">Taimera darbs tiek izpildīts, līdz tiek sinhronizētas izmaiņas.</span><span class="sxs-lookup"><span data-stu-id="931dd-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="931dd-107">Laiks, kas nepieciešams darba palaišanai, ir atkarīgs no procesa izmaiņu skaita.</span><span class="sxs-lookup"><span data-stu-id="931dd-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="931dd-108">Liels skaits izmaiņas ilgst ilgāk.</span><span class="sxs-lookup"><span data-stu-id="931dd-108">A large number of changes takes longer.</span></span> <span data-ttu-id="931dd-109">Pakalpojumu līmeņa līgums (SLA) norāda, ka izmaiņas lietotājam SharePoint Online direktorijā tiks atspoguļotas lietotāja profila lietojumprogrammu 24 stundu laikā.</span><span class="sxs-lookup"><span data-stu-id="931dd-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="931dd-110">Papildinformācija par lietotāja profila sinhronizācija SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="931dd-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

