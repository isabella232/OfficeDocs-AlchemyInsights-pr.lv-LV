---
title: Jautājumi par to, kā izmantot Office izvietošanas rīku (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 604fc200517316de6e0194bd64e6eb3039cfa61b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/18/2019
ms.locfileid: "36553547"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="55bba-102">Jautājumi par to, kā izmantot Office izvietošanas rīku (ODT)</span><span class="sxs-lookup"><span data-stu-id="55bba-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="55bba-103">Lejupielādējiet Office izvietošanas rīku no [Microsoft lejupielādes centra](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="55bba-103">Download the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="55bba-104">Pēc lejupielādes failu, palaidiet pašizpletes izpildāmo failu, kurā ir Office izvietošanas rīka izpildāmā (setup. exe) un parauga konfigurācijas failu (Configuration. XML).</span><span class="sxs-lookup"><span data-stu-id="55bba-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="55bba-105">**Lai izslēgtu vai noņemtu Office 365 ProPlus produktus no klientdatoriem:**</span><span class="sxs-lookup"><span data-stu-id="55bba-105">**To exclude or remove Office 365 ProPlus products from client computers:**</span></span>
  
<span data-ttu-id="55bba-106">Instalējot Office 365 ProPlus, varat izslēgt konkrētus produktus.</span><span class="sxs-lookup"><span data-stu-id="55bba-106">When installing Office 365 ProPlus, you can exclude specific products.</span></span> <span data-ttu-id="55bba-107">Lai to izdarītu, izpildiet Office instalēšanai ar ODT, bet ietver elementu ExcludeApp konfigurācijas failā.</span><span class="sxs-lookup"><span data-stu-id="55bba-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="55bba-108">Piemēram, šis konfigurācijas fails instalē visus Office 365 ProPlus produktus, izņemot Publisher:</span><span class="sxs-lookup"><span data-stu-id="55bba-108">For example, this configuration file installs all the Office 365 ProPlus products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="55bba-109">Pārskats par Office izvietošanas rīku</span><span class="sxs-lookup"><span data-stu-id="55bba-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

