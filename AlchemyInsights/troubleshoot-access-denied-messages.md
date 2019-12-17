---
title: Ziņojumu par piekļuvi liegta problēmu novēršana
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 05d12aee49b449e8a29e84021b41298fb9983859
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050712"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="8baee-102">Ziņojumu par piekļuvi liegta problēmu novēršana</span><span class="sxs-lookup"><span data-stu-id="8baee-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="8baee-103">Ja kāds ir ziņojums "piekļuve liegta" koplietojamo mapi SharePoint, vietņu kolekcijas administrators, iespējams, ir iespējota "ierobežotas piekļuves lietotāja atļaujas noslēgšanas režīmā."</span><span class="sxs-lookup"><span data-stu-id="8baee-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="8baee-104">Lai izslēgtu šo opciju:</span><span class="sxs-lookup"><span data-stu-id="8baee-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="8baee-105">Atrodiet vietni, noklikšķiniet uz ikonas iestatījumi un pēc tam noklikšķiniet uz **vietnes iestatījumi**.</span><span class="sxs-lookup"><span data-stu-id="8baee-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="8baee-106">Sadaļā **vietņu kolekcijas administrēšana**noklikšķiniet uz **vietņu kolekcijas līdzekļi**.</span><span class="sxs-lookup"><span data-stu-id="8baee-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="8baee-107">Blakus **ierobežotas piekļuves lietotāja atļaujas noslēgšanas režīmam**noklikšķiniet uz **deaktivizēt**.</span><span class="sxs-lookup"><span data-stu-id="8baee-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="8baee-108">Ziņojumu par liegtu piekļuvi var rasties arī koplietojamās mapes, ja vietne ir publicēšanas vietne.</span><span class="sxs-lookup"><span data-stu-id="8baee-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="8baee-109">Lai iegūtu informāciju, skatiet sadaļu [piekļuve liegta, piekļūstot koplietojamai mapei](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="8baee-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="8baee-110">Ja kāds ir saņēmis ziņojumu "piekļuve liegta", mēģinot skatīt piekļuves pieprasījumus, lietotājam ir jāpievieno kā vietņu kolekcijas administrators vai vietnes īpašnieku grupas dalībnieks.</span><span class="sxs-lookup"><span data-stu-id="8baee-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="8baee-111">Lai iegūtu papildinformāciju, skatiet [piekļuve liegta piekļuves pieprasījumu sarakstam](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="8baee-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="8baee-112">Ja lietotājs saņēma ziņojumu "piekļuve liegta" pēc tās noņemšanas no Active Directory lokālas un pēc tam pievienot atpakaļ, skatiet [piekļuve liegta, kad lietotāja konts ir sinhronizēts ar Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="8baee-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

