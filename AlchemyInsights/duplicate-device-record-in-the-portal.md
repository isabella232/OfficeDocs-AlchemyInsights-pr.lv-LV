---
title: Dublikāta ierīces ieraksts portālā
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 277afc59705e6040f0f9ae0c8cad965bd7d3ef65
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/23/2020
ms.locfileid: "43789868"
---
# <a name="duplicate-device-record-in-the-portal"></a>Dublikāta ierīces ieraksts portālā

Ja ierīce nepareizi ziņo par līdzpārvaldības statusu konfigurācijas pārvaldnieka vietnē, iespējams, būs redzami divi ieraksti ierīcei portālā. Lai pārbaudītu ierīces līdzpārvaldības statusu, pārskatiet ierīces **Līdzpārvaldības** kolonnu konfigurācijas pārvaldnieka konsolē. Ja kolonna nav redzama, varat to pievienot, ar peles labo pogu noklikšķinot uz jebkuras kolonnas galvenes un atlasot to sarakstā.

Vienlaikus pārvaldītajai vērtībai ir jābūt **Jā**. Ja vērtība ir **Nē**, atveriet konfigurācijas pārvaldnieka klienta sīklietotni klienta ierīcē un pārbaudiet, vai cilnē Vispārīgi **Līdzpārvaldības** rekvizītu.

- Ja vērtība ir **Iespējota**, tas norāda uz problēmām ar klienta saziņu ar pārvaldības punktu. Lūdzu, pārskatiet **CcmMessaging.log** ierīcē, lai izpētītu potenciālās savienojamības problēmas.

- Ja vērtība ir **Atspējota** un ierīce ir reģistrēta Intune, lūdzu, pārliecinieties, vai ierīce ir saņēmusi pārvaldības politiku, pārskatot **CoManagementHandler.log** ierīcē.
