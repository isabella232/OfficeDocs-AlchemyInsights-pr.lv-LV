---
title: Novērsiet DKIM uzstādīšanas kļūdas
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765219"
---
# <a name="fix-dkim-setup-issues"></a>Novērsiet DKIM uzstādīšanas kļūdas

Ja jums rodas problēmas, ļaujot DKIM pielāgoto domēnu, rīkojieties šādi:

- Visvairāk DKIM uzstādīšanas jautājumi ir saistīti ar nepareizu DNS ierakstus. Pārbaudiet, vai pareizi noformēta DKIM CNAME ieraksts (**nav** TXT ierakstu). Lai iegūtu papildinformāciju, skatiet šajā [tēmā](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

- Pēc tam, kad esat izveidot vai atjaunināt DKIM DNS ierakstu DNS viesošanas pakalpojumu savam domēnam (parasti, domēnu reģistrators), pagaidiet izplatīt DNS ierakstus.

- Ja jūs nevarat izveidot DKIM DNS ieraksti administrēšanas centrā, jūs varat nomainīt \<CustomDomain\> ar pielāgoto domēnu (piemēram, contoso.com) un palaist šo komandu [Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)PowerShell: `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.
