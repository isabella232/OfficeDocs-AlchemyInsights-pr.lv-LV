---
title: Automātisko atbilžu iestatīšana pastkastē
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: aeeb2e1e76fe602d2767b422797452fd1155fdd5
ms.sourcegitcommit: fdfd41c2bfb2d45003b3906e6469377384a91cb5
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2020
ms.locfileid: "43509508"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Automātisko atbilžu iestatīšana lietotāja pastkastē

**1. metode**

1. Pierakstieties Office 365 portālā.

2. Dodieties uz **Lietotāji > Aktīvie lietotāji** (vai **Grupas > Koplietojamās pastkastes**, ja esat iestatījis šo kā koplietojamo pastkasti).

3. Atlasiet lietotāju, kuram ir Microsoft Exchange pastkaste.

4. Uznirstošajā izvēlnē labajā pusē dodieties uz **Pasta iestatījumi > Automātiskās atbildes** (ja tā ir koplietojama pastkaste, vienkārši izvēlnē noklikšķiniet uz **Automātiskās atbildes**).

**2. metode**

1. Pierakstieties Office 365 administrēšanas portālā, izmantojot administratora akreditācijas datus.

2. Izvērsiet sadaļu **Administrēšanas centri** un pēc tam noklikšķiniet uz **Exchange**.

3. Noklikšķiniet uz attēla augšējā labajā stūrī, noklikšķiniet uz **Cits lietotājs** un pēc tam atlasiet lietotāja pastkasti, kuru vēlaties mainīt.

4. Kreisajā pusē atlasiet **Opcijas**, noklikšķiniet uz **Organizēt e-pastu** un pēc tam uz **Automātiskās atbildes.**

**3. metode**

Izpildiet tālāk norādīto cmdlet programmā Exchange Online PowerShell:

PowerShellCopy

```
    Set-MailboxAutoReplyConfiguration
```

Papildinformāciju par šo cmdlet komandu skatiet rakstā [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).
