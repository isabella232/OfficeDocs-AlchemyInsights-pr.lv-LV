---
title: E-pasta piegādes problēmu novēršana publiskajās mapēs, kurās iespējots pasts
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
- "1956"
- "3500007"
ms.openlocfilehash: ff1400f694ae037a8658356af068b4c20b8fa9d9908dafedb90db7bb6859530f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068819"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>E-pasta piegādes problēmu novēršana publiskajās mapēs, kurās iespējots pasts

Ja ārējie sūtītāji nevar nosūtīt ziņojumus uz publiskajām mapēm, kurās iespējots pasts, un sūtītāji saņem šādu kļūdu: nevarēja atrast **(550 5.4.1),** pārliecinieties, vai publiskās mapes e-pasta domēns ir konfigurēts kā iekšējās pārraides domēns, nevis autoritatīvs domēns:

1. Atveriet Exchange [administrēšanas centru (EAC).](https://docs.microsoft.com/Exchange/exchange-admin-center)

2. Dodieties **uz Pasta plūsma** \> **Akceptētie domēni**, atlasiet akceptēto domēnu un pēc tam noklikšķiniet uz **Rediģēt**.

3. Rekvizītu lapā, kas tiek atvērta, ja domēna tips ir iestatīts kā **Autoritatīvs,** mainiet vērtību uz **Iekšējā** pārraide un pēc tam noklikšķiniet uz **Saglabāt**.

Ja ārējie sūtītāji saņem kļūdu, jums nav atļaujas **(550 5.7.13),** izpildiet šādu komandu programmā [Exchange Online PowerShell,](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) lai skatītu atļaujas anonīmiem lietotājiem publiskajā mapē:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Piemēram, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Lai ļautu ārējiem lietotājiem nosūtīt e-pasta ziņojumus uz šo publisko mapi, pievienojiet CreateItems piekļuvi tieši lietotājam Anonīmam. Piemēram, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
