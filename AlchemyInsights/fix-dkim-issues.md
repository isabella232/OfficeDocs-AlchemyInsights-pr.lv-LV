---
title: DKIM uzstādīšanas problēmu labošana
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506781"
---
# <a name="fix-dkim-setup-issues"></a>DKIM uzstādīšanas problēmu labošana

Ja rodas problēmas, iespējojot DKIM pielāgotu domēnu, veiciet šādas darbības:

- Lielākā daļa DKIM uzstādīšanas problēmas ir saistītas ar nepareizu DNS ierakstus. Pārbaudiet DKIM CNAME ieraksts (**nav** txt ieraksts) ir formatēts pareizi. Lai iegūtu papildinformāciju, skatiet šo [tēmu](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- Pēc tam, kad izveidojat vai atjaunināt DKIM DNS ierakstu DNS viesošanas pakalpojumu domēna (parasti domēna reģistrētājs), uzgaidiet, kamēr tiek izplatīts DNS ierakstus.

- Ja nevarat izveidot DKIM DNS ierakstus administrēšanas centrs, varat aizstāt \<CustomDomain\> ar savu pielāgoto domēnu (piemēram, contoso.com) un palaist šo komandu [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
