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
description: Ja, aktivizējot programmu Office 2013 attālās darbvirsmas pakalpojumu (RDS) izvietojumos, tiek parādīts kļūdas ziņojums, apsveriet iespēju iespējot ADAL, rediģējot reģistru.
ms.openlocfilehash: ed3770c001461c162ff5bbe24dc400a29380a03b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316693"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Kļūda, aktivizējot Office 2013 attālās darbvirsmas pakalpojumos

Ja, aktivizējot programmu Office 2013 attālās darbvirsmas pakalpojumu (RDS) izvietojumos, tiek parādīts kļūdas ziņojums, apsveriet iespēju iespējot ADAL, rediģējot reģistru.
  
|**Reģistra atslēga**|**Tips**|**Vērtība**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Papildinformāciju skatiet rakstā [Modernās autentifikācijas iespējošana Office 2013 Windows ierīcēs](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
**Piezīme.** Programmā Microsoft 365 programmas lieluzņēmumiem 2016 ADAL Office pēc noklusējuma. Attālās darbvirsmas pakalpojumi (RdS) iepriekš tika nosaukti par Termināļa pakalpojumiem.
  