---
title: Automātisko atbilžu iestatīšana pastkastē
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 60af581e7fe508ab9644a53873bcd551b3aacff1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820941"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Automātisko atbilžu iestatīšana lietotāja pastkastē

**1. metode**

1. Pierakstieties programmas Microsoft 365 portālā.

2. Dodieties uz **Lietotāji > Aktīvie lietotāji** (vai **Grupas > Koplietojamās pastkastes**, ja esat iestatījis šo kā koplietojamo pastkasti).

3. Atlasiet lietotāju, kuram ir Microsoft Exchange pastkaste.

4. Uznirstošajā izvēlnē labajā pusē dodieties uz **Pasta iestatījumi > Automātiskās atbildes** (ja tā ir koplietojama pastkaste, vienkārši izvēlnē noklikšķiniet uz **Automātiskās atbildes**).

**2. metode**

1. Pierakstieties Microsoft 365 administrēšanas portālā, izmantojot administratora akreditācijas datus.

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
