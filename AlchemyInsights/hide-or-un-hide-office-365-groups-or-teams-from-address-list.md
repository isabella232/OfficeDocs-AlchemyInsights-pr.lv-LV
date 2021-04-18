---
title: Paslēpt vai parādīt Office 365 grupas vai darba grupas no adrešu saraksta
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
- "9002947"
- "5642"
ms.openlocfilehash: 12e221c69775f3dfeed1781b70d3061e1ca0ac3b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811463"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Paslēpt vai parādīt Office 365 grupas vai darba grupas no adrešu saraksta

Izmantojiet tālāk redzamo komandu EXO PowerShell komandu, lai paslēptu vai parādītu Office 365 grupas/darba grupas no Exchange klientu adrešu sarakstiem (GAL) (Outlook, OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Izmantojiet tālāk redzamo komandu EXO PowerShell, lai paslēptu vai parādītu Office365 grupas/darba grupas no Exchange klientiem (Outlook, OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Detalizētus norādījumus skatiet sadaļā [Paslēpt Office 365 grupas no GAL un Exchange klientiem](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).
