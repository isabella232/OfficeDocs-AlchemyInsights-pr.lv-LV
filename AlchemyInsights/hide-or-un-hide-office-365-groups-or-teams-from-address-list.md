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
ms.openlocfilehash: 7e667e22cd81f38a1a2c1385bf42e5227cb641480f4b505110ee7349a13f13a1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088403"
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
