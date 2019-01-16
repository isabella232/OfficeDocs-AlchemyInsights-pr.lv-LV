---
title: 1554 Winsock kļūda 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 96a9cfd11941158ddf13655c74974e3eb800e570
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/15/2019
ms.locfileid: "28300111"
---
# <a name="winsock-error-10061"></a>Winsock kļūda 10061

Šo kļūdas kodu, nozīmē, ka Office 365 nevarētu izveidot TCP ligzda (savienojums) ar mērķa resursdatoru. Visdrīzāk, ka cēlonis šīs kļūdas ir ar ugunsmūra konfigurāciju saistīta problēma. Lai novērstu problēmu, pārbaudiet šos iestatījumus:
  
- Pārbaudiet, vai jūsu ugunsmūra konfigurēšanu ar informāciju, kas atrodas [Office 365 URL un IP adrešu diapazons](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
    
- Ja kļūda ir specifiski uz Exchange Online aizsardzība (EOP), jums vajadzētu ir iepriekš paziņots [Exchange Online aizsardzība IP adreses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)maiņa.
    
- Pārliecinieties, ka jūsu interneta pakalpojumu sniedzēja (ISP) nav bloķē portu.
    
- Pārbaudiet, vai gudrs uzņēmējas un mērķa servera uzstādījumus jūsu savienotāji.
    
Ievērojiet, ka Office 365 nav bloķēt *ienākošos* savienojumus šādā veidā. 
  

