---
title: DKIM iestatīšanas problēmu novēršana
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744957"
---
# <a name="fix-dkim-setup-issues"></a>DKIM iestatīšanas problēmu novēršana

Ja rodas problēmas, kas sniedz DKIM savam pielāgotajam domēnam, veiciet tālāk norādītās darbības.

- Lielākā daļa DKIM iestatīšanas problēmu attiecas uz nepareiziem DNS ierakstiem. Pārbaudiet, vai DKIM CNAME ieraksts (**nevis** txt ieraksts) ir pareizi formatēts. Papildinformāciju skatiet šajā [tēmā](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- Pēc tam, kad esat izveidojis vai atjauninājis savus DKIM DNS ierakstus sava domēna DNS viesošanas pakalpojumā (parasti jūsu domēnu reģistrētājs), uzgaidiet, līdz tiek izplatīti DNS ieraksti.

- Ja nevarat izveidot DKIM DNS ierakstus administrēšanas centrā, varat aizstāt \<CustomDomain\> ar savu pielāgoto domēnu (piemēram, contoso.com) un izpildīt šo komandu pakalpojumā [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
