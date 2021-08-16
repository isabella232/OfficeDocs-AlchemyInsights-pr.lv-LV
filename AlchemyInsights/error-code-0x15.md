---
title: Kļūdas koda 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Ja tiek parādīts kļūdas ziņojums, aktivizējot Office 2013 attālās darbvirsmas pakalpojumu (RDS) izvietojumos, apsveriet iespēju iespējot ADAL, rediģējot reģistru.
ms.openlocfilehash: 247686bf26c11d07ed118bdb1ba190fc718e87cf140b88f79b8aa0b40c827b4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54100769"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Kļūda, aktivizējot Office 2013 attālās darbvirsmas pakalpojumos

Ja tiek parādīts kļūdas ziņojums, aktivizējot Office 2013 attālās darbvirsmas pakalpojumu (RDS) izvietojumos, apsveriet iespēju iespējot ADAL, rediģējot reģistru.
  
|**Reģistra atslēga**|**Tips**|**Vērtība**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Papildinformāciju skatiet rakstā [Modernās autentifikācijas iespējošana Office 2013 Windows ierīcēs](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL pēc noklusējuma ir iespējots programmā Microsoft 365 programmas lieluzņēmumiem 2016 Office. Attālās darbvirsmas pakalpojumi (RdS) iepriekš tika nosaukti par Termināļa pakalpojumiem.
  