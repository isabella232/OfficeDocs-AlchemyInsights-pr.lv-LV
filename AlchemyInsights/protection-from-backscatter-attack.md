---
title: Aizsardzība pret atstarojumu uzbrukumu
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036075"
---
# <a name="protection-from-backscatter-attack"></a>Aizsardzība pret atstarojumu uzbrukumu

Atstarojums ir atskaites par neizdevušos piegādi (tiek dēvētas arī par NDR vai Bounce ziņojumiem), ko saņemat ziņojumiem, kurus neesat nosūtījis. Surogātpasta izplatītāji Forge (mānīšanās) **:** to ziņojumu adresē, un tie bieži izmanto reālas e-pasta adreses, lai piešķirtu uzticību viņu ziņojumiem. Līdz ar to, kad surogātpasta sūtītāji nenovēršami sūta ziņojumus uz neesošiem adresātiem, mērķa e-pasta serveris būtībā tiek apkrāpts par nepiegādātu ziņojumu, kas tiek atgriezts NDR, uz viltoto sūtītāju **no:** adrese.

Papildu informācija ir atrodama sadaļā [atstarojums pakalpojumā EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).

**Iespējot atstarojumu aizsardzību**

Lai iespējotu atstarojumu aizsardzību, izpildiet tālāk esošo ceļu.

**protection.office.com > draudu pārvaldības > politikas > Antispam > atlasiet surogātpasta filtrēšanas politiku un rediģējiet politiku > surogātpasta rekvizītus > atzīmējiet kā surogātpasta > NDR atstarojums > iestatīt uz "ieslēgts"**

Ja uzskatāt, ka konts ir apdraudēts, skatiet tālāk minētos.

- [Atbildēšana uz e-pasta kontu](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [Bloķēto lietotāju noņemšana no ierobežotas lietotāju portāla pakalpojumā Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



