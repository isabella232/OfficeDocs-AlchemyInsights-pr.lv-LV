---
title: Jautājumi par to, kā lietot Office izvietošanas rīku (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: c16b7ac7d79794307fa33ed1039305ed5b842cf6
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/15/2019
ms.locfileid: "28299808"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="b7098-102">Jautājumi par to, kā lietot Office izvietošanas rīku (ODT)</span><span class="sxs-lookup"><span data-stu-id="b7098-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="b7098-103">Lejupielādējiet Office izvietošanas rīku no [Microsoft lejupielādes centra](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="b7098-103">Download the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="b7098-104">Pēc lejupielādes failu palaist pašizpletes izpildāmā faila, kurā atrodas Office izvietošanas rīku izpildāmā (setup.exe) un parauga konfigurācijas failu (Configuration).</span><span class="sxs-lookup"><span data-stu-id="b7098-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="b7098-105">**Izslēgt vai noņemt Office 365 ProPlus produktus no klientu datoriem:**</span><span class="sxs-lookup"><span data-stu-id="b7098-105">**To exclude or remove Office 365 ProPlus products from client computers:**</span></span>
  
<span data-ttu-id="b7098-p101">Instalējot Office 365 ProPlus, var neiekļaut konkrētu produktu. Lai to izdarītu, izpildiet Office instalēšanai ar ODT, bet iekļauj ExcludeApp elementu konfigurācijas failā. Piemēram, šis konfigurācijas failu instalē Office 365 ProPlus produktus, izņemot izdevējs:</span><span class="sxs-lookup"><span data-stu-id="b7098-p101">When installing Office 365 ProPlus, you can exclude specific products. To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file. For example, this configuration file installs all the Office 365 ProPlus products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="b7098-109">Pārskatu par Office ieviešanas rīks</span><span class="sxs-lookup"><span data-stu-id="b7098-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

