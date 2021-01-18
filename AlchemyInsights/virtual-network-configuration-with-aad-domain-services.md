---
title: Virtuālā konfigurācija ar AAD Domain Services
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885655"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>Virtuālā konfigurācija ar AAD Domain Services

Virtuālā konfigurācija ar AAD Domain Services ietver tālāk norādītās darbības. 

1. Domēna darbspējas pārbaude Azure portālā https://aka.ms/aadds-health
2. NSG pārbaude, vai nav tādu kārtulu, kas bloķē portus, kas nepieciešami, lai sinhronizētu Azure AD domēna pakalpojumos portālā https://aka.ms/aadds-networking
3. Pārliecinieties, vai jūsu virtuālais tīkls ir izvietots vienā Azure reģionā kā Azure AD Domain Services pārvaldītais domēns.
4. Nodrošināt, ka jums nav tāda domēna, kuram ir tāds pats domēna nosaukums, kas pieejams virtuālajā tīklā.

Lai iegūtu detalizētu informāciju par noformējuma atmaksu Azure virtuālajā tīklā, kas atbalsta AAD domēna pakalpojumus, skatiet rakstu [virtuālā tīkla uzmanība](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).

