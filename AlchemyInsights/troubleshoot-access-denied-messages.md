---
title: Piekļuve liegta ziņojumu novēršana
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 6c8ad84123fb58b73b9c378592ce970997893ea2
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704901"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="1d3f1-102">Piekļuve liegta ziņojumu novēršana</span><span class="sxs-lookup"><span data-stu-id="1d3f1-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="1d3f1-103">Ja kāds ir saņēmis ziņojumu "piekļuve liegta" koplietojamā mapē pakalpojumā SharePoint, vietņu kolekcijas administrators, iespējams, ir iespējojis "ierobežotas piekļuves lietotāju atļauju slēgšanas režīmu".</span><span class="sxs-lookup"><span data-stu-id="1d3f1-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="1d3f1-104">Lai izslēgtu šo līdzekli:</span><span class="sxs-lookup"><span data-stu-id="1d3f1-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="1d3f1-105">Pārlūkojiet līdz vietnei, noklikšķiniet uz ikonas Iestatījumi un pēc tam noklikšķiniet uz **vietnes iestatījumi**.</span><span class="sxs-lookup"><span data-stu-id="1d3f1-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="1d3f1-106">Sadaļā **vietņu kolekcijas administrēšana** noklikšķiniet uz **vietņu kolekcijas līdzekļi**.</span><span class="sxs-lookup"><span data-stu-id="1d3f1-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="1d3f1-107">Blakus opcijai **ierobežotas piekļuves lietotāju atļauju slēgšanas režīms** noklikšķiniet uz **deaktivizēt**.</span><span class="sxs-lookup"><span data-stu-id="1d3f1-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="1d3f1-108">Ja vietne ir publicēšanas vietne, koplietojamām mapēm var tikt parādīts arī ziņojums par liegtu piekļuvi.</span><span class="sxs-lookup"><span data-stu-id="1d3f1-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="1d3f1-109">Informāciju skatiet rakstā [piekļuve liegta, ja piekļūstat koplietojamai mapei](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span><span class="sxs-lookup"><span data-stu-id="1d3f1-109">For info, see [Access Denied when accessing a shared folder](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span></span>
  
<span data-ttu-id="1d3f1-110">Ja kāds ir saņēmis ziņojumu "piekļuve liegta", kad mēģināt skatīt piekļuves pieprasījumus, lietotājs ir jāpievieno kā vietņu kolekcijas administrators vai vietnes īpašnieku grupas dalībnieks.</span><span class="sxs-lookup"><span data-stu-id="1d3f1-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="1d3f1-111">Papildinformāciju skatiet rakstā [piekļuve liegta piekļuves pieprasījumu sarakstam](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="1d3f1-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="1d3f1-112">Ja lietotājam ir noņemts ziņojums "piekļuve liegta" pēc tam, kad tie tika noņemti no lokālā Active Directory un pēc tam atkal pievienots, skatiet sadaļu [piekļuve liegta, kad lietotāja konts ir sinhronizēts ar Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="1d3f1-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

