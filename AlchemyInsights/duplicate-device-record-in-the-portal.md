---
title: Dublikāta ierīces ieraksts portālā
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
- "9001495"
- "4386"
ms.openlocfilehash: e6f477807823e68965ce966faf0a6f50f9472f3d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814523"
---
# <a name="duplicate-device-record-in-the-portal"></a>Dublikāta ierīces ieraksts portālā

Ja ierīce nepareizi ziņo par līdzpārvaldības statusu konfigurācijas pārvaldnieka vietnē, iespējams, būs redzami divi ieraksti ierīcei portālā. Lai pārbaudītu ierīces līdzpārvaldības statusu, pārskatiet ierīces **Līdzpārvaldības** kolonnu konfigurācijas pārvaldnieka konsolē. Ja kolonna nav redzama, varat to pievienot, ar peles labo pogu noklikšķinot uz jebkuras kolonnas galvenes un atlasot to sarakstā.

Vienlaikus pārvaldītajai vērtībai ir jābūt **Jā**. Ja vērtība ir **Nē**, atveriet konfigurācijas pārvaldnieka klienta sīklietotni klienta ierīcē un pārbaudiet, vai cilnē Vispārīgi **Līdzpārvaldības** rekvizītu.

- Ja vērtība ir **Iespējota**, tas norāda uz problēmām ar klienta saziņu ar pārvaldības punktu. Lūdzu, pārskatiet **CcmMessaging.log** ierīcē, lai izpētītu potenciālās savienojamības problēmas.

- Ja vērtība ir **Atspējota** un ierīce ir reģistrēta Intune, lūdzu, pārliecinieties, vai ierīce ir saņēmusi pārvaldības politiku, pārskatot **CoManagementHandler.log** ierīcē.
