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
ms.openlocfilehash: e9f7581fd21cf5ca2d712038c4b73b67d08f3a76
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774898"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Jautājumi par to, kā izmantot Office izvietošanas rīku (ODT)

Lejupielādējiet Office izvietošanas rīku no [Microsoft lejupielādes centra](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Pēc faila lejupielādes palaidiet izpildāmo failu, kurā ir iekļauts Office izvietošanas rīks (setup.exe) un parauga konfigurācijas failu (configuration.xml).
  
 **Lai izslēgtu vai noņemtu Microsoft 365 lietojumprogrammas darbam ar Enterprise produktiem no klienta datoriem:**
  
Instalējot Microsoft 365 lietojumprogrammas uzņēmumam, varat izslēgt noteiktus produktus. Lai to paveiktu, izpildiet darbības, lai instalētu Office, izmantojot ODT, bet iekļaujiet ExcludeApp elementu konfigurācijas failā. Piemēram, šajā konfigurācijas failā tiek instalētas visas Microsoft 365 lietojumprogrammas darbam ar Enterprise produktiem, izņemot Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Pārskats par Office izvietošanas rīku](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

