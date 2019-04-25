---
title: Profilu sinhronizācijas
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: d1a72a85767e36fefbfa8eee266befcaf2e48af0
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/23/2019
ms.locfileid: "32371991"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="07d7b-102">Kad manu profilu izmaiņas sinhronizēt pieteikumu SharePoint lietotāja profilu?</span><span class="sxs-lookup"><span data-stu-id="07d7b-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="07d7b-103">SharePoint Online izmanto Active Directory importēšana taimera darbu (AD importa) importēt lietotāja profila programmu lietotājiem un grupām.</span><span class="sxs-lookup"><span data-stu-id="07d7b-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="07d7b-104">Reklāmu importa sinhronizē izmaiņas no SharePoint Online Directory Store pieteikumu lietotāja profilu.</span><span class="sxs-lookup"><span data-stu-id="07d7b-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="07d7b-105">Šīs izmaiņas tiek apstrādāti tikai partijas.</span><span class="sxs-lookup"><span data-stu-id="07d7b-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="07d7b-106">Taimera darbu vada, līdz tiek sinhronizētas izmaiņas.</span><span class="sxs-lookup"><span data-stu-id="07d7b-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="07d7b-107">Laiks, kas paiet veicamo darbu, ir atkarīgs no izmaiņu procesu skaits.</span><span class="sxs-lookup"><span data-stu-id="07d7b-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="07d7b-108">Lielu skaitu izmaiņas prasa ilgāku laiku.</span><span class="sxs-lookup"><span data-stu-id="07d7b-108">A large number of changes takes longer.</span></span> <span data-ttu-id="07d7b-109">Pakalpojuma līmeņa vienošanās (SLA) norāda, ka 24 stundu laikā mainīt SharePoint Online Directory lietotājam tiks atspoguļotas programmu lietotāja profilu.</span><span class="sxs-lookup"><span data-stu-id="07d7b-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="07d7b-110">Vairāk info par lietotāju profila sinhronizācijas SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="07d7b-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

