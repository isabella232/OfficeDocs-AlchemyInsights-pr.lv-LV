---
title: Saglabāt jūsu mājas lapā ar savu pašreizējo hostinga sniedzēja DNS ieraksti tiks atjaunināti
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: f2cdb319e56b82c09b7a9856c81a45e69dee6759
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/23/2019
ms.locfileid: "32423730"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="7a42f-102">Saglabāt jūsu mājas lapā ar savu pašreizējo hostinga sniedzēja DNS ieraksti tiks atjaunināti</span><span class="sxs-lookup"><span data-stu-id="7a42f-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="7a42f-103">Lapā [Domēni](https://portal.office.com/adminportal/home#/Domains) domēnu, sarakstā atlasiet domēna jūs izmantojat jūsu mājas lapā un pēc tam atlasiet **DNS iestatījumus** rūts vadība.</span><span class="sxs-lookup"><span data-stu-id="7a42f-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website, and then select **DNS settings** in the management pane.</span></span> 
    
2. <span data-ttu-id="7a42f-104">Atlasiet **+ jaunu pielāgotu ierakstu** un ievadiet šādu formulu:</span><span class="sxs-lookup"><span data-stu-id="7a42f-104">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="7a42f-105">Ievadiet **DNS tips** : **(adrese)**</span><span class="sxs-lookup"><span data-stu-id="7a42f-105">For **DNS type** enter: **A (Address)**</span></span>
    
  - <span data-ttu-id="7a42f-106">**Resursdatora nosaukumu vai aizstājvārdu**, ievadiet:**@**</span><span class="sxs-lookup"><span data-stu-id="7a42f-106">For **Host name or Alias**, type the following: **@**</span></span>
    
  - <span data-ttu-id="7a42f-107">**IP adresi**, ierakstiet statiska IP adrese jūsu mājas lapā, kur tas pašlaik ir izvietots (piemēram, 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="7a42f-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span> 
    
    <span data-ttu-id="7a42f-108">Šim ir jābūt *statiskā* IP adrese tīmekļa vietni, nevis *dinamisko* IP adresi.</span><span class="sxs-lookup"><span data-stu-id="7a42f-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="7a42f-109">Sazinieties ar vietu, kur jūsu mājas lapā tiek izvietots, lai pārliecinātos, jūs varat saņemt statisko IP adresi jūsu publiskajā vietnē.</span><span class="sxs-lookup"><span data-stu-id="7a42f-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span> 
    
3. <span data-ttu-id="7a42f-110">Izvēlieties **Saglabāt**.</span><span class="sxs-lookup"><span data-stu-id="7a42f-110">Select **Save**.</span></span> 
    
<span data-ttu-id="7a42f-111">Turklāt varat izveidot CNAME ierakstu, lai palīdzētu klientiem atrast jūsu mājas lapā.</span><span class="sxs-lookup"><span data-stu-id="7a42f-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="7a42f-112">Atlasiet **+ jaunu pielāgotu ierakstu** un ievadiet šādu formulu:</span><span class="sxs-lookup"><span data-stu-id="7a42f-112">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="7a42f-113">Ievadiet **DNS tips** : **CNAME (aizstājvārds)**</span><span class="sxs-lookup"><span data-stu-id="7a42f-113">For **DNS type** enter: **CNAME (Alias)**</span></span>
    
  - <span data-ttu-id="7a42f-114">**Resursdatora nosaukumu vai aizstājvārdu**, rakstiet sekojošo: **www**</span><span class="sxs-lookup"><span data-stu-id="7a42f-114">For **Host name or Alias**, type the following: **www**</span></span>
    
  - <span data-ttu-id="7a42f-115">**Norāda uz adresi**, ievadiet pilnībā kvalificētu domēna nosaukumu (FQDN) jūsu mājas lapā (piemēram, contoso.com).</span><span class="sxs-lookup"><span data-stu-id="7a42f-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span> 
    
2. <span data-ttu-id="7a42f-116">Izvēlieties **Saglabāt**.</span><span class="sxs-lookup"><span data-stu-id="7a42f-116">Select **Save**.</span></span> 
    

