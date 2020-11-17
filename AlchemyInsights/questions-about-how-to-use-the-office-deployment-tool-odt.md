---
title: Jautājumi par to, kā izmantot Office izvietošanas rīku (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: c5b055989014b464d3136895702c8ea40e8eb701
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086163"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="c6488-102">Jautājumi par to, kā izmantot Office izvietošanas rīku (ODT)</span><span class="sxs-lookup"><span data-stu-id="c6488-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="c6488-103">Lejupielādējiet Office izvietošanas rīku no [Microsoft lejupielādes centra](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="c6488-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="c6488-104">Pēc faila lejupielādes palaidiet izpildāmo failu, kurā ir iekļauts Office izvietošanas rīks (setupodt.exe) un parauga konfigurācijas failu (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="c6488-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setupodt.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="c6488-105">**Lai izslēgtu vai noņemtu Microsoft 365 lietojumprogrammas darbam ar Enterprise produktiem no klienta datoriem:**</span><span class="sxs-lookup"><span data-stu-id="c6488-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="c6488-106">Instalējot Microsoft 365 lietojumprogrammas uzņēmumam, varat izslēgt noteiktus produktus.</span><span class="sxs-lookup"><span data-stu-id="c6488-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="c6488-107">Lai to paveiktu, izpildiet darbības, lai instalētu Office, izmantojot ODT, bet iekļaujiet ExcludeApp elementu konfigurācijas failā.</span><span class="sxs-lookup"><span data-stu-id="c6488-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="c6488-108">Piemēram, šajā konfigurācijas failā tiek instalētas visas Microsoft 365 lietojumprogrammas darbam ar Enterprise produktiem, izņemot Publisher:</span><span class="sxs-lookup"><span data-stu-id="c6488-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="c6488-109">Pārskats par Office izvietošanas rīku</span><span class="sxs-lookup"><span data-stu-id="c6488-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

