---
title: Jautājumi par to, kā izmantot Office izvietošanas rīku (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 96d3f70f554f71c43d6458ec8debc099cd9fb040
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43698065"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Jautājumi par to, kā izmantot Office izvietošanas rīku (ODT)

Lejupielādējiet Office izvietošanas rīku no [Microsoft lejupielādes centra](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Pēc lejupielādes failu, palaidiet pašizpletes izpildāmo failu, kurā ir Office izvietošanas rīka izpildāmā (setup. exe) un parauga konfigurācijas failu (Configuration. XML).
  
 **Lai izslēgtu vai noņemtu Microsoft 365 lietojumprogrammas uzņēmuma produktiem no klientdatoriem:**
  
Instalējot Microsoft 365 lietojumprogrammas uzņēmumiem, varat izslēgt konkrētu produktu. Lai to izdarītu, izpildiet Office instalēšanai ar ODT, bet ietver elementu ExcludeApp konfigurācijas failā. Piemēram, šis konfigurācijas fails instalē visas Microsoft 365 lietojumprogrammas uzņēmuma produktiem, izņemot Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Pārskats par Office izvietošanas rīku](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

