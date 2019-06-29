---
title: 1554 Winsock kļūda 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e82e90b670235848105636fb2039ed60d3b93c67
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/28/2019
ms.locfileid: "35364920"
---
# <a name="winsock-error-10061"></a>Winsock kļūda 10061

Šo kļūdas kodu, nozīmē, ka Office 365 nevarētu izveidot TCP ligzda (savienojums) ar mērķa resursdatoru. Visdrīzāk, ka cēlonis šīs kļūdas ir ar ugunsmūra konfigurāciju saistīta problēma. Lai novērstu problēmu, pārbaudiet šos iestatījumus:

- Pārbaudiet, vai jūsu ugunsmūra konfigurēšanu ar informāciju, kas atrodas [Office 365 URL un IP adrešu diapazons](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Ja kļūda ir specifiski uz Exchange Online aizsardzība (EOP), jums vajadzētu ir iepriekš paziņots [Exchange Online aizsardzība IP adreses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)maiņa.

- Pārliecinieties, ka jūsu interneta pakalpojumu sniedzēja (ISP) nav bloķē portu.

- Pārbaudiet, vai gudrs uzņēmējas un mērķa servera uzstādījumus jūsu savienotāji.

Ievērojiet, ka Office 365 nav bloķēt *ienākošos* savienojumus šādā veidā.
