---
title: E-pasta piegādes problēmu novēršana pasta publiskajām mapēm
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716359"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>E-pasta piegādes problēmu novēršana pasta publiskajām mapēm

Ja ārējie sūtītāji nevar nosūtīt ziņojumus uz jūsu pasta publiskajām mapēm un sūtītāji saņem kļūdas ziņojumu: **nevarēja atrast (550 5.4.1)**, pārbaudiet, vai publiskās mapes e-pasta domēns ir konfigurēts kā iekšējais pārraides domēns, nevis autoritatīvs domēns:

1. Atveriet [Exchange administrēšanas centru (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Dodieties uz **pasta plūsma** \> **akceptēts domēnu**, atlasiet **akceptētun**pēc tam noklikšķiniet uz Rediģēt.

3. Rekvizītu lapā, kas tiek atvērts, ja domēna tips ir iestatīts uz **autoritatīvs**, mainiet vērtību uz **iekšējo pārraidi** un pēc tam noklikšķiniet uz **saglabāt**.

Ja ārējie sūtītāji saņem kļūdas **jums nav atļaujas (550 5.7.13)**, izpildiet šādu komandu [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) , lai redzētu anonīmo lietotāju atļaujas publiskajā mapē:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Piemēram, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Lai atļautu ārējiem lietotājiem nosūtīt e-pasta ziņojumu uz šo publisko mapi, pievienojiet CreateItems piekļuves tiesības lietotājam anonīms. Piemēram, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
