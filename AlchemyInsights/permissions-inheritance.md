---
title: Atļauju pārmantošana
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bb5c440a-ca70-4dc6-b517-688e80551101
ms.openlocfilehash: f086bd7312772b399146cd81261f147364d64665
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741958"
---
# <a name="how-permissions-inheritance-works-in-sharepoint"></a><span data-ttu-id="76bb7-102">Kā atļauju pārmantošana darbojas koplietošanas vidē SharePoint</span><span class="sxs-lookup"><span data-stu-id="76bb7-102">How permissions inheritance works in SharePoint</span></span>

<span data-ttu-id="76bb7-103">Pēc noklusējuma hierarhiskā vidē SharePoint atļaujas tiek pārmantotas augstāk.</span><span class="sxs-lookup"><span data-stu-id="76bb7-103">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="76bb7-104">Tādējādi fails pārmanto atļaujas no mapes, kas pārmanto atļaujas no bibliotēkas, kas pārmanto atļaujas no vietnes, kas pārmanto atļaujas no vietņu kolekcijas.</span><span class="sxs-lookup"><span data-stu-id="76bb7-104">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site, which inherits its permissions from the site collection.</span></span>
  
<span data-ttu-id="76bb7-105">Informāciju par unikālu atļauju noņemšanu un pārmantošanas atjaunošanu skatiet rakstā [saraksta vai bibliotēkas atļauju rediģēšana un pārvaldība](https://go.microsoft.com/fwlink/?linkid=869946).</span><span class="sxs-lookup"><span data-stu-id="76bb7-105">For info about removing unique permissions and restoring inheritance, see [Edit and manage permissions for a list or library](https://go.microsoft.com/fwlink/?linkid=869946).</span></span>
  

