---
title: Profila sinhronizācija
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: eee1080a95955332e205db3852381e39aaf5ae0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801776"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="777a9-102">Kad mans profils maina sinhronizāciju ar SharePoint lietotāja profila lietojumprogrammu?</span><span class="sxs-lookup"><span data-stu-id="777a9-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="777a9-103">SharePoint Online izmanto Active Directory importēšanas taimera darbu (AD Import), lai lietotājus un grupas importētu lietotāju profilu lietojumprogrammā.</span><span class="sxs-lookup"><span data-stu-id="777a9-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="777a9-104">AD Import sinhronizē izmaiņas no SharePoint Online direktorija krātuves lietotāja profila lietojumprogrammā.</span><span class="sxs-lookup"><span data-stu-id="777a9-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="777a9-105">Šīs izmaiņas tiek apstrādātas partijās.</span><span class="sxs-lookup"><span data-stu-id="777a9-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="777a9-106">Taimera darbs tiek izpildīts līdz brīdim, kad tiek sinhronizētas izmaiņas.</span><span class="sxs-lookup"><span data-stu-id="777a9-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="777a9-107">Darba izpildes laiks ir atkarīgs no procesa izmaiņu skaita.</span><span class="sxs-lookup"><span data-stu-id="777a9-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="777a9-108">Lielākam skaitam izmaiņu ir nepieciešams ilgāks laiks.</span><span class="sxs-lookup"><span data-stu-id="777a9-108">A large number of changes takes longer.</span></span> <span data-ttu-id="777a9-109">Pakalpojumu līmeņa līgumā (SLA) ir norādīts, ka izmaiņas lietotājam SharePoint Online direktorijā tiks atspoguļotas lietotāja profila lietojumprogrammā 24 stundu laikā.</span><span class="sxs-lookup"><span data-stu-id="777a9-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="777a9-110">Papildinformācija par lietotāju profilu sinhronizāciju pakalpojumā SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="777a9-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

