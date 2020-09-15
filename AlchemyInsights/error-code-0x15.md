---
title: Kļūdas kods 0x15
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
description: Ja, aktivizējot Office 2013 attālā datora pakalpojumu (RDS) izvietojumā, rodas kļūda, apsveriet iespēju iespējot ADAL, rediģējot reģistru.
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709194"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Kļūda, aktivizējot Office 2013 attālās darbvirsmas pakalpojumos

Ja, aktivizējot Office 2013 attālā datora pakalpojumu (RDS) izvietojumā, rodas kļūda, apsveriet iespēju iespējot ADAL, rediģējot reģistru.
  
|**Reģistra atslēga**|**Ierakstiet**|**Vērtību**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Lai iegūtu papildinformāciju, skatiet rakstu [modernās autentifikācijas iespējošana pakalpojumā Office 2013 Windows ierīcēs](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL ir iespējota pēc noklusējuma Microsoft 365 programmās darbam ar Enterprise un Office 2016. Attālā datora pakalpojumu (RDS) iepriekš tika nosaukts termināļa pakalpojumi.
  