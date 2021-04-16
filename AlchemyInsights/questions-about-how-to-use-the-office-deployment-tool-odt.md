---
title: Jautājumi par To, kā izmantot Office izvietošanas rīku (ODT)
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 20e0b6aa3c298ee0a4291c3da6ae46978177e81f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790339"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="d74a1-102">Jautājumi par To, kā izmantot Office izvietošanas rīku (ODT)</span><span class="sxs-lookup"><span data-stu-id="d74a1-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="d74a1-103">Lejupielādējiet Office izvietošanas rīku no [Microsoft lejupielādes centra](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="d74a1-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="d74a1-104">Pēc faila lejupielādes palaidiet izpildāmo failu, kas satur izpildāmo Office izvietošanas rīku (setup.exe) un konfigurācijas faila paraugu (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="d74a1-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="d74a1-105">**Lai klientu datoros izslēgtu vai noņemtu Microsoft 365 lietojumprogrammas uzņēmumiem:**</span><span class="sxs-lookup"><span data-stu-id="d74a1-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="d74a1-106">Instalējot Microsoft 365 lietojumprogrammas uzņēmumiem, varat izslēgt konkrētus produktus.</span><span class="sxs-lookup"><span data-stu-id="d74a1-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="d74a1-107">Lai to izdarītu, izpildiet darbības, kas jāveic, lai instalētu Office, izmantojot ODT, bet iekļaut elementu ExcludeApp savā konfigurācijas failā.</span><span class="sxs-lookup"><span data-stu-id="d74a1-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="d74a1-108">Piemēram, šis konfigurācijas fails instalē visus Microsoft 365 programmu uzņēmumu produktus, izņemot Publisher:</span><span class="sxs-lookup"><span data-stu-id="d74a1-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="d74a1-109">Office izvietošanas rīka pārskats</span><span class="sxs-lookup"><span data-stu-id="d74a1-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

