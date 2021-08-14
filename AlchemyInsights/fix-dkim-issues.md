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
ms.openlocfilehash: 5a613321ed79e657350ec4d19b1f07ac0a091b227a8268c793a10edd9990d41f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945938"
---
# <a name="fix-dkim-setup-issues"></a>DKIM iestatīšanas problēmu novēršana

Ja rodas problēmas, iespējojot DKIM jūsu pielāgotajam domēnam, veiciet tālāk norādītās darbības.

- Lielākā daļa DKIM iestatīšanas problēmu ir saistītas ar nepareiziem DNS ierakstiem. Pārbaudiet, vai DKIM CNAME ieraksts **(nevis** TXT ieraksts) ir pareizi formatēts. Papildinformāciju skatiet šajā [tēmā](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- Kad esat izveidojis vai atjauninījis DKIM DNS ierakstus jūsu domēnam (parasti jūsu domēnu reģistrētājam) DNS viesošanas pakalpojumā, uzgaidiet, līdz DNS ieraksti tiek izplatīti.

- Ja nevarat izveidot DKIM DNS ierakstus administrēšanas centrā, varat aizstāt ar savu pielāgoto domēnu (piemēram, contoso.com) un izpildīt šo komandu programmā \<CustomDomain\> [Exchange Online PowerShell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
