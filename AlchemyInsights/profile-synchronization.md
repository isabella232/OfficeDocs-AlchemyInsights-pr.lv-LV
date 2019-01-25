---
title: Profilu sinhronizācijas
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: a32cf9e623d1be7a2c85ef4951c6eb7f001b7db0
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/24/2019
ms.locfileid: "29479784"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="7160f-102">Kad manu profilu izmaiņas sinhronizēt pieteikumu SharePoint lietotāja profilu?</span><span class="sxs-lookup"><span data-stu-id="7160f-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="7160f-103">SharePoint Online izmanto Active Directory importēšana taimera darbu (AD importa) importēt lietotāja profila programmu lietotājiem un grupām.</span><span class="sxs-lookup"><span data-stu-id="7160f-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="7160f-p101">Reklāmu importa sinhronizē izmaiņas no SharePoint Online Directory Store pieteikumu lietotāja profilu. Šīs izmaiņas tiek apstrādāti tikai partijas.</span><span class="sxs-lookup"><span data-stu-id="7160f-p101">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application. These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="7160f-106">Taimera darbu vada, līdz tiek sinhronizētas izmaiņas.</span><span class="sxs-lookup"><span data-stu-id="7160f-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="7160f-p102">Laiks, kas paiet veicamo darbu, ir atkarīgs no izmaiņu procesu skaits. Lielu skaitu izmaiņas prasa ilgāku laiku. Pakalpojuma līmeņa vienošanās (SLA) norāda, ka 24 stundu laikā mainīt SharePoint Online Directory lietotājam tiks atspoguļotas programmu lietotāja profilu.</span><span class="sxs-lookup"><span data-stu-id="7160f-p102">The time it takes the job to run depends on the number of changes to process. A large number of changes takes longer. The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="7160f-110">Vairāk info par lietotāju profila sinhronizācijas SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="7160f-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

