---
title: Jautājumi par to, kā izmantot Office izvietošanas rīku (ODT)
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
ms.openlocfilehash: d38866647c7bf286b5b5b21e7fdcc94af72ea1850bc40391af077aa230b8b4fd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959690"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Jautājumi par to, kā izmantot Office izvietošanas rīku (ODT)

Lejupielādējiet Office 2016 izvietošanas rīku [no Microsoft lejupielādes centra.](https://go.microsoft.com/fwlink/p/?LinkID=626065)
  
Pēc faila lejupielādes palaidiet izpildāmo failu, kas satur izpildāmo Office izvietošanas rīka izpildāmo failu (setup.exe) un konfigurācijas faila paraugu (configuration.xml).
  
 **Lai klienta datoros Microsoft 365 programmas lieluzņēmumiem vai noņemtu šos produktus:**
  
Instalējot Microsoft 365 programmas lieluzņēmumiem, varat izslēgt konkrētus produktus. Lai to izdarītu, izpildiet norādītās darbības, lai instalētu Office ar ODT, bet iekļaujiet excludeapp elementu savā konfigurācijas failā. Piemēram, šis konfigurācijas fails instalē visus Microsoft 365 programmas lieluzņēmumiem produktus, izņemot Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Pārskats par Office izvietošanas rīku](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

