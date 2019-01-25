---
title: Kļūdas kods 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Ja saņemat kļūdas, vienlaikus aktivizējot Office 2013 attālās darbvirsmas pakalpojumu (RDS) izvietošanās, apsveriet iespēju aktivizēt ADAL, rediģējot reģistru.
ms.openlocfilehash: 89f9270169e13fd7706f7826c624ef8ae4d47b3f
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499389"
---
Ja saņemat kļūdas, vienlaikus aktivizējot Office 2013 attālās darbvirsmas pakalpojumu (RDS) izvietošanās, apsveriet iespēju aktivizēt ADAL, rediģējot reģistru. 
  
|**Reģistra atslēga**| adreses joslā ierakstiet |Vērtība|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |
   
Papildinformāciju skatiet sadaļā [Iespējot modernās autentifikācijas Office tips skaitlim 2013 Windows ierīcēs](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL ir iespējota pēc noklusējuma Office 365 ProPlus un biroja 2016. > attālās darbvirsmas pakalpojumu (RDS) iepriekš tika nosaukts Terminal Services. 
  

