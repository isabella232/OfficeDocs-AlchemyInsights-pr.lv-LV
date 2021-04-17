---
title: DNS ierakstu atjaunināšana, lai savu tīmekļa vietni uzturētu ar pašreizējo viesošanas pakalpojumu sniedzēju
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 89bce2aa5931c0c20706efabd42d2351be43938b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827532"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="13d4c-102">DNS ierakstu atjaunināšana, lai savu tīmekļa vietni uzturētu ar pašreizējo viesošanas pakalpojumu sniedzēju</span><span class="sxs-lookup"><span data-stu-id="13d4c-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="13d4c-103">Microsoft 365 administrēšanas centrā dodieties uz lapu Domēnu iestatīšana un domēnu sarakstā atlasiet tīmekļa vietnei  >  lietoto domēnu.[](https://admin.microsoft.com/Adminportal#/Domains)</span><span class="sxs-lookup"><span data-stu-id="13d4c-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://admin.microsoft.com/Adminportal#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="13d4c-104">Atlasiet **+ Jauns pielāgots ieraksts** un ievadiet:</span><span class="sxs-lookup"><span data-stu-id="13d4c-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="13d4c-105">Sadaļā **DNS tips** ievadiet A **(adrese)**</span><span class="sxs-lookup"><span data-stu-id="13d4c-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="13d4c-106">Laukā **Resursdatora nosaukums vai aizstājvārds** ierakstiet šādu tekstu: **@**</span><span class="sxs-lookup"><span data-stu-id="13d4c-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="13d4c-107">Laukā **IP adrese** ierakstiet statisko IP adresi, kur pašlaik tiek viesota jūsu tīmekļa vietne (piemēram, 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="13d4c-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="13d4c-108">Tai ir jābūt  *statiskai tīmekļa*  vietnes IP adresei, nevis  *dinamiskajai*  IP adresei.</span><span class="sxs-lookup"><span data-stu-id="13d4c-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="13d4c-109">Pārbaudiet vietni, kur tiek viesota jūsu tīmekļa vietne, lai pārliecinātos, vai varat iegūt statisku IP adresi jūsu publiskaajai tīmekļa vietnei.</span><span class="sxs-lookup"><span data-stu-id="13d4c-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="13d4c-110">Atlasiet **Saglabāt**.</span><span class="sxs-lookup"><span data-stu-id="13d4c-110">Select **Save**.</span></span>

<span data-ttu-id="13d4c-111">Turklāt varat izveidot CNAME ierakstu, lai klientiem palīdzētu atrast jūsu tīmekļa vietni.</span><span class="sxs-lookup"><span data-stu-id="13d4c-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="13d4c-112">Atlasiet **+ Jauns pielāgots ieraksts** un ievadiet:</span><span class="sxs-lookup"><span data-stu-id="13d4c-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="13d4c-113">Sadaļā **DNS tips ievadiet** **CNAME (aizstājvārds)**</span><span class="sxs-lookup"><span data-stu-id="13d4c-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="13d4c-114">Laukā **Resursdatora nosaukums vai aizstājvārds** ierakstiet šādu informāciju: **www**</span><span class="sxs-lookup"><span data-stu-id="13d4c-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="13d4c-115">Laukā **Norāda uz** adresi ierakstiet savas tīmekļa vietnes pilno domēna nosaukumu (FQDN) (piemēram, contoso.com).</span><span class="sxs-lookup"><span data-stu-id="13d4c-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="13d4c-116">Atlasiet **Saglabāt**.</span><span class="sxs-lookup"><span data-stu-id="13d4c-116">Select **Save**.</span></span>
