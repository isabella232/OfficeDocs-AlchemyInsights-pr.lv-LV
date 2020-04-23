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
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717569"
---
# <a name="fix-dkim-setup-issues"></a>DKIM uzstādīšanas problēmu labošana

Ja rodas problēmas, iespējojot DKIM pielāgotu domēnu, veiciet šādas darbības:

- Lielākā daļa DKIM uzstādīšanas problēmas ir saistītas ar nepareizu DNS ierakstus. Pārbaudiet DKIM CNAME ieraksts (**nav** txt ieraksts) ir formatēts pareizi. Lai iegūtu papildinformāciju, skatiet šo [tēmu](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

- Pēc tam, kad izveidojat vai atjaunināt DKIM DNS ierakstu DNS viesošanas pakalpojumu domēna (parasti domēna reģistrētājs), uzgaidiet, kamēr tiek izplatīts DNS ierakstus.

- Ja nevarat izveidot DKIM DNS ierakstus administrēšanas centrs, varat \<aizstāt customdomain\> ar savu pielāgoto domēnu (piemēram, contoso.com) un palaist šo komandu [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell):. `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`
