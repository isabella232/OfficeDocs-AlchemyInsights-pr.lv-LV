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
ms.openlocfilehash: af7085890d295cf0c41e11aaf18e404313413100cb8a1134bfac051d5fa26996
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53926252"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Paslēpt Microsoft 365 grupu no adrešu saraksta (GAL)

Lai paslēptu Microsoft 365 grupu no Exchange klientu (piemēram, Outlook vai OWA) adrešu sarakstiem (GAL), EXO čaulā izmantojiet šādu komandu:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Lai paslēptu Microsoft 365 grupu, lai tā Exchange klientiem, izmantojiet šādu komandu EXO čaulā:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

