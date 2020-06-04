---
title: Atjauniniet DNS ierakstus, lai uzturētu jūsu vietni ar pašreizējo viesošanas pakalpojumu sniedzēju
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 7bd36c3954d12d3ee4ac624a2f827d8e5cd88082
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665767"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="bbd4c-102">Atjauniniet DNS ierakstus, lai uzturētu jūsu vietni ar pašreizējo viesošanas pakalpojumu sniedzēju</span><span class="sxs-lookup"><span data-stu-id="bbd4c-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="bbd4c-103">Microsoft 365 administrēšanas centrā pārejiet uz lapu **iestatījumu**  >  [Domēni](https://portal.office.com/adminportal/home#/Domains) un domēnu sarakstā atlasiet domēnu, kuru izmantojat savai vietnei.</span><span class="sxs-lookup"><span data-stu-id="bbd4c-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://portal.office.com/adminportal/home#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="bbd4c-104">Atlasiet **+ Jauns pielāgots ieraksts** un ievadiet sekojošo:</span><span class="sxs-lookup"><span data-stu-id="bbd4c-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="bbd4c-105">**DNS tipa** ievadei: **a (adrese)**</span><span class="sxs-lookup"><span data-stu-id="bbd4c-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="bbd4c-106">**Resursdatora nosaukumu vai aizstājvārdu**, ierakstiet šādu:**@**</span><span class="sxs-lookup"><span data-stu-id="bbd4c-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="bbd4c-107">Lai iegūtu **IP adresi**, ierakstiet savas vietnes statisko IP adresi, kur tā pašlaik tiek viesota (piemēram, 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="bbd4c-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="bbd4c-108">Šī ir *statiska* IP adrese mājas lapā, nevis *dinamisko* IP adresi.</span><span class="sxs-lookup"><span data-stu-id="bbd4c-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="bbd4c-109">Pārbaudiet ar vietni, kur jūsu mājas lapā ir izvietots, lai pārliecinātos, ka jūs varat saņemt statisku IP adresi jūsu publiskajā vietnē.</span><span class="sxs-lookup"><span data-stu-id="bbd4c-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="bbd4c-110">Atlasiet **saglabāt**.</span><span class="sxs-lookup"><span data-stu-id="bbd4c-110">Select **Save**.</span></span>

<span data-ttu-id="bbd4c-111">Turklāt varat izveidot CNAME ierakstu, lai palīdzētu klientiem atrast jūsu vietni.</span><span class="sxs-lookup"><span data-stu-id="bbd4c-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="bbd4c-112">Atlasiet **+ Jauns pielāgots ieraksts** un ievadiet sekojošo:</span><span class="sxs-lookup"><span data-stu-id="bbd4c-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="bbd4c-113">**DNS tipa** ievadiet: **CNAME (aizstājvārds)**</span><span class="sxs-lookup"><span data-stu-id="bbd4c-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="bbd4c-114">**Resursdatora nosaukumu vai aizstājvārdu**, ierakstiet šādu: **www**</span><span class="sxs-lookup"><span data-stu-id="bbd4c-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="bbd4c-115">Par **punktiem, uz adresi**, ierakstiet pilnu domēna nosaukumu (FQDN) jūsu mājas lapā (piemēram, contoso.com).</span><span class="sxs-lookup"><span data-stu-id="bbd4c-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="bbd4c-116">Atlasiet **saglabāt**.</span><span class="sxs-lookup"><span data-stu-id="bbd4c-116">Select **Save**.</span></span>
