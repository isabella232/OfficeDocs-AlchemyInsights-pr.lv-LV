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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Jautājumi par to, kā izmantot Office izvietošanas rīku (ODT)

Lejupielādējiet Office izvietošanas rīku no [Microsoft lejupielādes centra](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Pēc lejupielādes failu, palaidiet pašizpletes izpildāmo failu, kurā ir Office izvietošanas rīka izpildāmā (setup. exe) un parauga konfigurācijas failu (Configuration. XML).
  
 **Lai izslēgtu vai noņemtu Office 365 ProPlus produktus no klientdatoriem:**
  
Instalējot Office 365 ProPlus, varat izslēgt konkrētus produktus. Lai to izdarītu, izpildiet Office instalēšanai ar ODT, bet ietver elementu ExcludeApp konfigurācijas failā. Piemēram, šis konfigurācijas fails instalē visus Office 365 ProPlus produktus, izņemot Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Pārskats par Office izvietošanas rīku](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

