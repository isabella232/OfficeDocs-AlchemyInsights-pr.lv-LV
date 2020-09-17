---
title: DNS ierakstu atjaunināšana, lai savu tīmekļa vietni uzturētu ar pašreizējo viesošanas pakalpojumu sniedzēju
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 1d8654bc2dfb9063d0203992d624285eb646027d
ms.sourcegitcommit: 78939b01579b626b147d356045a37aec1170c948
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47815792"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="908e5-102">DNS ierakstu atjaunināšana, lai savu tīmekļa vietni uzturētu ar pašreizējo viesošanas pakalpojumu sniedzēju</span><span class="sxs-lookup"><span data-stu-id="908e5-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="908e5-103">Microsoft 365 administrēšanas centrā dodieties uz lapu **iestatīšanas**  >  [Domēni](https://admin.microsoft.com/Adminportal#/Domains) un domēnu sarakstā atlasiet tīmekļa vietnei izmantojamo domēnu.</span><span class="sxs-lookup"><span data-stu-id="908e5-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://admin.microsoft.com/Adminportal#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="908e5-104">Atlasiet **+ Jauns pielāgots ieraksts** un ievadiet šādu informāciju:</span><span class="sxs-lookup"><span data-stu-id="908e5-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="908e5-105">Sadaļā **DNS tips** ievadiet: **a (adrese)**</span><span class="sxs-lookup"><span data-stu-id="908e5-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="908e5-106">Sadaļā **resursdatora nosaukums vai aizstājvārds**ierakstiet šādu informāciju: **@**</span><span class="sxs-lookup"><span data-stu-id="908e5-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="908e5-107">Sadaļā **IP adrese**ierakstiet statisko IP adresi savai tīmekļa vietnei, kur tā pašlaik tiek viesota (piemēram, 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="908e5-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="908e5-108">Šai tīmekļa vietnei ir jābūt  *statiskai*  IP adresei, nevis  *dinamiskajai*  IP adresei.</span><span class="sxs-lookup"><span data-stu-id="908e5-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="908e5-109">Lai pārliecinātos, vai jūsu publiskajai tīmekļa vietnei varat iegūt statisku IP adresi, skatiet vietni, kurā tiek viesota jūsu tīmekļa vietne.</span><span class="sxs-lookup"><span data-stu-id="908e5-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="908e5-110">Atlasiet **Saglabāt**.</span><span class="sxs-lookup"><span data-stu-id="908e5-110">Select **Save**.</span></span>

<span data-ttu-id="908e5-111">Turklāt varat izveidot CNAME ierakstu, lai klientiem palīdzētu atrast jūsu tīmekļa vietni.</span><span class="sxs-lookup"><span data-stu-id="908e5-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="908e5-112">Atlasiet **+ Jauns pielāgots ieraksts** un ievadiet šādu informāciju:</span><span class="sxs-lookup"><span data-stu-id="908e5-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="908e5-113">Sadaļā **DNS tips** ievadiet **CNAME (aizstājvārds)**</span><span class="sxs-lookup"><span data-stu-id="908e5-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="908e5-114">Sadaļā **resursdatora nosaukums vai aizstājvārds**ierakstiet šādu informāciju: **www**</span><span class="sxs-lookup"><span data-stu-id="908e5-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="908e5-115">**Punktos uz adresi**ierakstiet savas tīmekļa vietnes pilno domēna nosaukumu (FQDN) (piemēram, contoso.com).</span><span class="sxs-lookup"><span data-stu-id="908e5-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="908e5-116">Atlasiet **Saglabāt**.</span><span class="sxs-lookup"><span data-stu-id="908e5-116">Select **Save**.</span></span>
