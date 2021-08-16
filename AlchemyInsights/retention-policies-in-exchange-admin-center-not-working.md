---
title: Saglabāšanas politikas Exchange administrēšanas centrā nedarbojas
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 6652ad5fc1691e1d5a4293d81f3a649f23ec38f18c8ed9fe06665628a901d13e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074939"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Saglabāšanas politikas Exchange centrā

Ja vēlaties, lai mēs automatizēti veiktu tālāk minēto iestatījumu pārbaudes, atlasiet pogu Atpakaļ <- šīs lapas augšdaļā un pēc tam ievadiet tā lietotāja e-pasta adresi, kuram ir problēmas ar saglabāšanas politikām.

Ja rodas problēmas ar saglabāšanas politikām Exchange administrēšanas centrā, kas netiek lietots pastkastēm vai vienumiem, kas nepārvieto uz arhīva pastkasti, pārbaudiet šādus elementus:

**Saknes iemesli:**

- **Pārvaldītais mapes** palīgs nav apstrādājis lietotāja pastkasti. Pārvaldīto mapju palīgs ik pēc septiņām dienām mēģina apstrādāt katru pastkasti jūsu mākoņa organizācijā.

  **Risinājums:** Palaidiet pārvaldīto mapju palīgu.

- Pastkastē ir **iespējota opcija** **RetentionHold.** Ja pastkaste ir novietota saglabāšanas vietā, saglabāšanas politika pastkastē šajā laikā netiks apstrādāta.

  **Risinājums:** Pārbaudiet saglabāšanas aizturēšanas iestatījuma statusu un atjauniniet pēc nepieciešamības. Detalizētu informāciju skatiet rakstā [Pastkastes saglabāšanas aizturēšana.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)
 
**Piezīme.** Ja pastkaste ir mazāka par 10 MB, pārvaldīto mapju palīgs automātiski neapstrādā pastkasti.
 
Papildinformāciju par saglabāšanas politikām Exchange centrā skatiet:

- [Saglabāšanas atzīmes un saglabāšanas politikas](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Saglabāšanas politikas izmantošana pastkastēm vai Saglabāšanas](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) [tagu pievienošana vai noņemšana](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Pastkastes aizturēšanas veida identificēšana](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
