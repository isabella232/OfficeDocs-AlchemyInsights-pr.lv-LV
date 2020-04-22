---
title: Kļūdas kods 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Ja saņemat kļūdas ziņojumu, aktivizējot Office 2013 attālās darbvirsmas pakalpojumu (RDS) izvietošanu, apsveriet iespēju iespējot ADAL, rediģējot reģistru.
ms.openlocfilehash: 566d63cbe37d295b3546b9d7d5b14dfc8e8fe0ec
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703145"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Kļūda, aktivizējot Office 2013 attālās darbvirsmas pakalpojumos

Ja saņemat kļūdas ziņojumu, aktivizējot Office 2013 attālās darbvirsmas pakalpojumu (RDS) izvietošanu, apsveriet iespēju iespējot ADAL, rediģējot reģistru.
  
|**Reģistra atslēgu**|**Tipa**|**Vērtību**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |Reg_dword  <br/> |1  <br/> |

Lai iegūtu papildinformāciju, skatiet [Iespējot mūsdienu autentifikācijas Office 2013 Windows ierīcēs](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL ir iespējota pēc noklusējuma Microsoft 365 lietojumprogrammas Enterprise un Office 2016. Attālās darbvirsmas pakalpojumu (RDS) iepriekš tika nosaukts termināļa pakalpojumus.
  