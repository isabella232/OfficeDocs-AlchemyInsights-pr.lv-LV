---
title: 2491 brīdinājuma e-pasta ziņojumus no "phish piegādāts nomnieka vai lietotāja apiešanas dēļ" politika
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e4efd504304da757687e697ff23374aeea31851
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758935"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Alert e-pasta ziņojumus no "phish piegādāts dēļ nomnieka vai lietotāja ignorēt" politika

Noklusējuma brīdinājuma politika ar nosaukumu "phish piegādāts nomnieka vai lietotāja apiešanas dēļ" ir tika izvelēta nomniekiem ar Office 365 ATP P1 un P2 licencēm. Ja saņēmāt šo brīdinājumu, tālāk ir norādītas darbības, kas jāveic, lai izpētītu:

1. Brīdinājuma ziņojumā noklikšķiniet uz **Skatīt brīdinājumu** , lai drošības & atbilstības centrā pārietu uz lapu **brīdinājumi** .

2. Atlasiet brīdinājumu, lai skatītu opciju skatīt **ziņojumu sarakstu** vai **skatītu ziņojumus programmā Explorer**. Abas šīs opcijas ļauj piekļūt ziņojuma detaļām, kas ietver ziņojuma ID. Ņemiet vērā, ka saite Threat Explorer automātiski filtrē ziņojumus, kas atbilst brīdinājuma kritērijiem. Iespējams, ir jāpielāgo datuma filtrs Threat Explorer.

Pikšķerēšanas ziņojums tika piegādāts dēļ manuāli konfigurēta ignorēšana:

- Atļauto sūtītāju vai domēnu, ko iestatījis lietotājs.

- Atļauto sūtītāju vai domēnu, ko administrators iestatījis pretsurogātpasta politikā.

- Atļauto IP adresi savienojuma filtra politikā.

- Pasta plūsmas kārtula (tiek dēvēta arī par transportēšanas kārtulu), kas ir konfigurēta, lai atļautu ziņojumus.

Ja uzskatāt, ka ziņojums ir nepareizi atzīmēts kā phish, izmantojiet Outlook ziņojumu [ziņojumu pievienojumprogrammu](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) iesniegt ziņojumu paraugi Microsoft.
