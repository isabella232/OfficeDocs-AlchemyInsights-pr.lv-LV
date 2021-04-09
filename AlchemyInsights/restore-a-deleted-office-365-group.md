---
title: Izdzēstas Microsoft 365 grupas atjaunošana
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: b72b7c93ce9fe1b90d1608811b0eeabc8aec1363
ms.sourcegitcommit: a5edaaefdc56f8d5c8220a335f4e8228e2de4ee0
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/08/2021
ms.locfileid: "51645138"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Izdzēstas Microsoft 365 grupas atjaunošana

Izdzēstu Microsoft 365 grupu vai Microsoft Teams varat atjaunot 30 dienu laikā pēc dzēšanas.

1. Dodieties uz [Microsoft 365 administrēšanas](https://aka.ms/RestoreDeletedGroup) centru, lai pieteiktos sarakstā, kurā esat izdzēstās grupas un darba grupas.

    **Piezīme.** Piesakieties, izmantojot kontu, kas ir piešķirts nomnieka administratoram vai grupu administratora lomai.

1. Atlasiet izdzēsto Microsoft 365 grupu/grupu, kas jāatjauno, un noklikšķiniet **uz Atjaunot grupu**.

    Ja grupu nevar atjaunot konfliktējošas SMTP adreses dēļ, izmantojiet tālāk norādīto komandu, lai atrastu objektu, kas izraisa konfliktu, un noņemtu SMTP adresi:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Piezīme.** Dažos gadījumos grupas un visu tās datu atjaunošana var ilgt līdz pat 24 stundām.

    Lai iegūtu papildinformāciju vai uzzinātu, kā atjaunot grupas, izmantojot PowerShell, skatiet rakstu [Izdzēstas Microsoft 365 grupas atjaunošana.](https://go.microsoft.com/fwlink/?linkid=867802)