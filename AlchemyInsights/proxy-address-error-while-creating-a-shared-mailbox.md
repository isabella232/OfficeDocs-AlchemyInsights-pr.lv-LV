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
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568297"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Starpniekservera adreses kļūda, veidojot pastkasti vai citu e-pasta objektu

Ja mēģinājāt izveidot e-pasta objektu (pastkaste, koplietojama pastkaste utt.) un tiek parādīts kļūdas ziņojums "starpniekservera adrese" SMTP:alias@domain.com "jau tiek izmantota...", jūsu izvēlētajā e-pasta adresē jau ir cits e-pasta objekts jūsu organizācijā.
  
Jums ir jāatrod lietotāja, grupas, koplietojamas pastkastes vai publiskas mapes, kurā ir šī e-pasta adrese, vai jādzēš tā vai jāmaina tās e-pasta adrese. Pēc tam varat izveidot jaunu e-pasta objektu ar atbrīvoto e-pasta adresi. Lai to atrastu, sākumlapā izmantojiet meklēšanu. Varat arī izmantot šādu komandu Exchange Online PowerShell, lai to meklētu:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Ja nevēlaties dzēst esošo e-pasta adresi, izvēlieties jaunu e-pasta adresi jaunajam objektam, ko veidojat.
  