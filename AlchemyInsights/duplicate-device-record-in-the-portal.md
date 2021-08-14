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
ms.openlocfilehash: 7eb642f85f437fe216c49ce6b060c9061b477629fbd45f50ca0ef315b8cd32d3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004161"
---
# <a name="duplicate-device-record-in-the-portal"></a>Dublikāta ierīces ieraksts portālā

Ja ierīce nepareizi ziņo par līdzpārvaldības statusu konfigurācijas pārvaldnieka vietnē, iespējams, būs redzami divi ieraksti ierīcei portālā. Lai pārbaudītu ierīces līdzpārvaldības statusu, pārskatiet ierīces **Līdzpārvaldības** kolonnu konfigurācijas pārvaldnieka konsolē. Ja kolonna nav redzama, varat to pievienot, ar peles labo pogu noklikšķinot uz jebkuras kolonnas galvenes un atlasot to sarakstā.

Vienlaikus pārvaldītajai vērtībai ir jābūt **Jā**. Ja vērtība ir **Nē**, atveriet konfigurācijas pārvaldnieka klienta sīklietotni klienta ierīcē un pārbaudiet, vai cilnē Vispārīgi **Līdzpārvaldības** rekvizītu.

- Ja vērtība ir **Iespējota**, tas norāda uz problēmām ar klienta saziņu ar pārvaldības punktu. Lūdzu, pārskatiet **CcmMessaging.log** ierīcē, lai izpētītu potenciālās savienojamības problēmas.

- Ja vērtība ir **Atspējota** un ierīce ir reģistrēta Intune, lūdzu, pārliecinieties, vai ierīce ir saņēmusi pārvaldības politiku, pārskatot **CoManagementHandler.log** ierīcē.
