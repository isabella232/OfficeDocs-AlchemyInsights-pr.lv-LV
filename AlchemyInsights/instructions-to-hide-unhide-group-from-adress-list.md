---
title: Instructions to hide/unhide group from address list
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 4d55866700b9b8494f1f692cd3b865116b96a1bc
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831885"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Paslēpt Microsoft 365 grupu no adrešu saraksta (GAL)

Lai paslēptu Microsoft 365 grupu no Exchange klientu adrešu sarakstiem (GAL) (piemēram, Outlook vai OWA), EXO čaulā izmantojiet šādu komandu:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Lai paslēptu Microsoft 365 grupu, kas nav redzama Exchange klientiem, izmantojiet šādu komandu EXO čaulā:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

