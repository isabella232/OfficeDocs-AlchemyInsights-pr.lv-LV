---
title: Noteikt e-pasta piegādes jautājumiem pasta publiskajās mapēs
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 900b6cc2765937ee005c7e7dce5d33bbdf582601
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752676"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Noteikt e-pasta piegādes jautājumiem pasta publiskajās mapēs

Ja ārējiem sūtītājiem ziņas nevar nosūtīt pasta publiskajām mapēm un sūtītāju atgriezta kļūda: **nav atrodama (550 5.4.1)**, pārbaudīt e-pasta adreses domēns, lai publiskā mape ir konfigurēta kā iekšējo pārraides domēnu, nevis autoritatīvu domēnu:

1. Atveriet [Exchange administratoru centrā (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Dodieties uz **pasta plūsmu** \> **akceptēts domēni**atlasiet akceptēto domēnu un pēc tam noklikšķiniet uz **Rediģēt**.

3. Rekvizītu lapa kas tiek atvērts, ja domēna tips ir iestatīts kā **Authoritative**, mainiet vērtību uz **iekšējo pārraides** un pēc tam noklikšķiniet uz **Saglabāt**.

Ja ārējiem sūtītājiem saņemtu, **jums nav atļaujas (550 5.7.13)** kļūda, palaidiet tālāk norādīto komandu [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) , lai redzētu, kādas atļaujas par anonīmiem lietotājiem publiskajā mapē.

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Piemēram, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Ļaut ārējiem lietotājiem sūtīt e-pastu uz šo publisko mapi, pievienot CreateItems piekļuves tiesības anonīms lietotājs. Piemēram, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
