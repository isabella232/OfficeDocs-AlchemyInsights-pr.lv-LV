---
title: Jautājumi par to, kā lietot Office izvietošanas rīku (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: e91d40f872dd401ee210ac05eb39d64b6fb88027
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/12/2019
ms.locfileid: "29925351"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Jautājumi par to, kā lietot Office izvietošanas rīku (ODT)

Lejupielādējiet Office izvietošanas rīku no [Microsoft lejupielādes centra](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Pēc lejupielādes failu palaist pašizpletes izpildāmā faila, kurā atrodas Office izvietošanas rīku izpildāmā (setup.exe) un parauga konfigurācijas failu (Configuration).
  
 **Izslēgt vai noņemt Office 365 ProPlus produktus no klientu datoriem:**
  
Instalējot Office 365 ProPlus, var neiekļaut konkrētu produktu. Lai to izdarītu, izpildiet Office instalēšanai ar ODT, bet iekļauj ExcludeApp elementu konfigurācijas failā. Piemēram, šis konfigurācijas failu instalē Office 365 ProPlus produktus, izņemot izdevējs:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Pārskatu par Office ieviešanas rīks](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

