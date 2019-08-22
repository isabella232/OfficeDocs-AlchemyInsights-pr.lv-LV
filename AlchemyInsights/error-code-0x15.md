---
title: Kļūdas kods 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Ja saņemat kļūdas, vienlaikus aktivizējot Office 2013 attālās darbvirsmas pakalpojumu (RDS) izvietošanās, apsveriet iespēju aktivizēt ADAL, rediģējot reģistru.
ms.openlocfilehash: 4ef2943e5a529368fa2c614e4431cf180924fbb8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527021"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Attālās darbvirsmas pakalpojumu biroja 2013 aktivizēšanu, radās kļūda

Ja saņemat kļūdas, vienlaikus aktivizējot Office 2013 attālās darbvirsmas pakalpojumu (RDS) izvietošanās, apsveriet iespēju aktivizēt ADAL, rediģējot reģistru.
  
|**Reģistra atslēga**|**Tips**|**Vērtība**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Papildinformāciju skatiet sadaļā [Iespējot modernās autentifikācijas Office tips skaitlim 2013 Windows ierīcēs](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL ir iespējota pēc noklusējuma Office 365 ProPlus un biroja 2016. Attālās darbvirsmas pakalpojumu (RDS) iepriekš tika nosaukts Terminal Services.
  