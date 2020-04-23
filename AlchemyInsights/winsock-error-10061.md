---
title: 1554 Winsock kļūda 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766176"
---
# <a name="winsock-error-10061"></a>Winsock kļūda 10061

Šis kļūdas kods nozīmē, ka Microsoft nevarēja izveidot TCP ligzdu (savienojums) ar mērķa resursdatoru. Visticamākais šīs kļūdas cēlonis ir ugunsmūra konfigurācijas problēma. Lai novērstu šo problēmu, pārbaudiet šos iestatījumus:

- Pārbaudiet, vai ugunsmūra konfigurācija ar informāciju [Microsoft 365 URL un IP adrešu diapazoni](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Ja šī kļūda ir specifiska Exchange Online Protection (EOP), iepriekš tika paziņots izmaiņas [Exchange Online Protection IP adreses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Pārbaudiet, vai jūsu interneta pakalpojumu sniedzējs (ISP) nebloķē portu.

- Pārbaudiet, vai viedā resursdatora un mērķa servera iestatījumus jūsu savienotāji.

Ņemiet vērā, ka Microsoft 365 nebloķē *ienākošos* savienojumus šādā veidā.
