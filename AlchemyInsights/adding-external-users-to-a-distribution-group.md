---
title: Ārējo lietotāju pievienošana adresātu grupai
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663520"
---
# <a name="add-external-users-to-a-distribution-group"></a>Ārējo lietotāju pievienošana adresātu grupai

Ārējas kontaktpersonas pievienošana adresātu grupai (DG) ir divu soļu process:
  
1. Izveidojiet pasta kontaktpersonu ārējam lietotājam:
    
    1. Administrēšanas centrā dodieties uz lapu **lietotāju**  >  [kontaktpersonas](https://admin.microsoft.com/adminportal/home#/Contact) . 
    
    2. Atlasiet **Pievienot kontaktpersonu**.
    
    3. Ierakstiet kontaktpersonas informāciju un atlasiet **Pievienot**.
    
2. Pievienojiet pasta kontaktpersonu savam ĢENERĀLDIREKTORĀTAm:
    
    1. Administrēšanas centrā dodieties uz lapu **grupu**  >  [grupas](https://admin.microsoft.com/adminportal/home#/groups) . 
    
    2. Atrodiet DG, kuram vēlaties pievienot ārējo lietotāju, un atlasiet to, lai atvērtu rediģēšanas dialoglodziņu.
    
    3. Cilnē **dalībnieki** atlasiet **Skatīt visus un pārvaldīt dalībniekus**. 
    
    4. Atlasiet **Pievienot dalībniekus**.
    
    5. Atlasiet iepriekšējā darbībā izveidoto pasta kontaktpersonu un pēc tam atlasiet **Saglabāt**.
    
Ja pēc šo darbību veikšanas ārējie lietotāji nevar nosūtīt e-pasta ziņojumus uz DG vai nesaņem e-pasta ziņojumus no šīs darbības, iespējams, ka DG ir atzīmēts atļaut tikai e-pasta ziņojumus no iekšējiem lietotājiem. Varat pārbaudīt šo konfigurāciju un izlabot to, sekojot norādījumiem, kas sniegti [šeit](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Piezīme:** Šīs instrukcijas nav spēkā, ja jūsu grupas tips ir "Microsoft 365 Group", nevis "adresātu grupa". Šādā gadījumā ārējo lietotāju varat pievienot tieši grupai no Outlook. Detalizētu informāciju par Microsoft 365 grupām viesi, kā arī norādījumus par ārējo viesu pievienošanu, var skatīt [šajā rakstā](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  