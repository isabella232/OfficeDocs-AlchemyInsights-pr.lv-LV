---
title: 1554 Winsock kļūda 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 7991f83a0b4791eaa7eb3246f7e61f781e4c7430931fbf920d7fd9e44c018d13
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083237"
---
# <a name="winsock-error-10061"></a>Winsock kļūda 10061

Šis kļūdas kods nozīmē, ka Microsoft nevarēja izveidot TCP drošligzdu (savienojumu) ar mērķa resursdatoru. Visdrīzāk šīs kļūdas cēlonis ir problēma ar jūsu ugunsmūra konfigurāciju. Lai novērstu šo problēmu, pārbaudiet šos iestatījumus:

- Ugunsmūra konfigurācijas pārbaude ar informāciju, kas norādīta [Microsoft 365 URL un IP adrešu diapazonos](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Ja kļūda attiecas tieši uz Exchange Online Protection (EOP), jums iepriekš būtu jābūt informētiem par izmaiņām ip [Exchange Online Protection adresēs.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

- Pārbaudiet, vai jūsu interneta pakalpojumu sniedzējs (ISP) nebloķē portu.

- Pārbaudiet viedā resursdatora un mērķa servera iestatījumus savienotājos.

Ņemiet vērā Microsoft 365 ienākošie *savienojumi netiek* bloķēti šādā veidā.
