---
title: Starpniekservera adreses kļūda koplietojamas pastkastes izveides laikā
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: 7c15d5db5445fbe4c3ec22878f180f48d2da4f90369f2e6f223916646eb19c12
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54062915"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Starpniekservera adreses kļūda, izveidojot pastkasti vai citu objektu ar iespējotu e-pastu

Ja mēģinājāt izveidot e-pasta objektu (pastkasti, koplietojamu pastkasti utt.) un saņēmāt kļūdas ziņojumu "Starpniekservera adrese "SMTP:alias@domain.com" jau tiek izmantota...", jūsu izvēlēto e-pasta adresi jūsu organizācijā jau izmanto cits objekts, kurā iespējots e-pasts.
  
Atrodiet lietotāju, grupu, koplietojamo pastkasti vai publisko mapi, kurā ir šī e-pasta adrese, un izdzēsiet to vai mainiet tās e-pasta adresi. Pēc tam varat izveidot jaunu e-pasta objektu ar atbrīvoto e-pasta adresi. Izmantojiet meklēšanu sākumlapā, lai to atrastu. Lai to meklētu, Exchange Online šo PowerShell komandu:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Ja nevēlaties dzēst esošo e-pasta adresi, izvēlieties jaunu e-pasta adresi jaunajam objektam, kuru veidojat.
  