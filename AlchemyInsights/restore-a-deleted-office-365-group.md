---
title: Izdzēstas Microsoft 365 atjaunošana
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
ms.openlocfilehash: 6262ca04335c355fb4de41a9e1d854b666f47e10321a843717d6eb951c46cafd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959033"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Izdzēstas Microsoft 365 atjaunošana

Izdzēstu ziņojumu var Microsoft 365 grupas vai Microsoft Teams 30 dienu laikā pēc dzēšanas.

1. Dodieties [uz Microsoft 365 administrēšanas centrs,](https://aka.ms/RestoreDeletedGroup) lai pieteiktos sarakstā, kurā esat izdzēstās grupas un grupas.

    **Piezīme.** Piesakieties, izmantojot kontu, kas ir piešķirts nomnieka administratoram vai grupu administratora lomai.

1. Atlasiet izdzēsto Microsoft 365/Teams atjaunot un noklikšķiniet uz **Atjaunot grupu.**

    Ja grupu nevar atjaunot konfliktējošas SMTP adreses dēļ, izmantojiet tālāk norādīto komandu, lai atrastu objektu, kas izraisa konfliktu, un noņemtu SMTP adresi:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Piezīme.** Dažos gadījumos grupas un visu tās datu atjaunošana var ilgt līdz pat 24 stundām.

    Lai iegūtu papildinformāciju vai uzzinātu, kā atjaunot grupas, izmantojot PowerShell, skatiet [rakstu Izdzēstas grupas Microsoft 365 atjaunošana.](https://go.microsoft.com/fwlink/?linkid=867802)