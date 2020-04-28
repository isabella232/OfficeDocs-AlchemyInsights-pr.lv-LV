---
title: Ārējo lietotāju pievienošanu adresātu grupai
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 7dbc69bced9ca800d3f95081b77dda5e49662579
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/27/2020
ms.locfileid: "43910939"
---
# <a name="add-external-users-to-a-distribution-group"></a>Ārējo lietotāju pievienošana adresātu grupai

Ārēja kontakta pievienošana adresātu grupai (DG) ir divpakāpju process:
  
1. Ārējā lietotāja pasta kontaktpersonas izveide:
    
    1. Administrēšanas centrā atveriet lapu **lietotāju** > [kontaktpersonas](https://admin.microsoft.com/adminportal/home#/Contact) . 
    
    2. Atlasiet **Pievienot kontaktpersonu**.
    
    3. Ierakstiet kontaktpersonas informāciju un atlasiet **pievienot**.
    
2. Pievienot pasta kontaktpersona jūsu ĢD:
    
    1. Administrēšanas centrā pārejiet uz lapu **grupu** > [grupas.](https://admin.microsoft.com/adminportal/home#/groups) 
    
    2. Atrodiet ĢD, kuram vēlaties pievienot ārējo lietotāju, un atlasiet to, lai atvērtu rediģēšanas dialogu.
    
    3. Cilnē **dalībnieki** atlasiet **Skatīt visu un pārvaldīt dalībniekus**. 
    
    4. Atlasiet vienumu **pievienot dalībniekus**.
    
    5. Atlasiet iepriekšējā solī izveidoto pasta kontaktpersonu un pēc tam atlasiet **saglabāt**.
    
Ja pēc šīs darbības jūsu ārējie lietotāji nevar nosūtīt e-pastus DG vai nesaņem e-pastus no tā, tas varētu būt, ka ĢD ir atzīmēts atļaut tikai e-pastus no iekšējiem lietotājiem. Jūs varat pārbaudīt šo konfigurāciju un noteikt to pēc virzienos [šeit](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Piezīme:** Šīs instrukcijas neattiecas, ja grupas tips ir "Microsoft 365 grupas" nevis "adresātu grupas". Šādā gadījumā ārējo lietotāju var pievienot tieši grupai no programmas Outlook. Detalizēta informācija par Microsoft 365 grupām viesi, kā arī instrukcijas, lai pievienotu ārējos viesi var atrast [šajā rakstā](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  