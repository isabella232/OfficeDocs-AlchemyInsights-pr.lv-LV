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
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698869"
---
# <a name="winsock-error-10061"></a>Winsock kļūda 10061

Šis kļūdas kods nozīmē, ka Microsoft nevar izveidot TCP ligzdu (savienojumu) ar mērķi resursdators. Visticamāk, šīs kļūdas cēlonis ir problēmas ar ugunsmūra konfigurāciju. Lai novērstu šo problēmu, pārbaudiet šos iestatījumus:

- Ugunsmūra konfigurācijas pārbaudīšana, izmantojot informāciju [Microsoft 365 vietrāžus URL un IP adrešu diapazonos](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Ja kļūda ir specifiska Exchange Online Protection (EOP), jums ir iepriekš jāziņo par izmaiņām [Exchange Online Protection IP adresēs](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Pārbaudiet, vai jūsu interneta pakalpojumu sniedzējs (ISP) nebloķē portu.

- Pārliecinieties, vai jūsu savienotājiem ir gudri resursdators un mērķserveri iestatījumi.

Ņemiet vērā, ka Microsoft 365 nebloķē *ienākošos* savienojumus šādā veidā.
