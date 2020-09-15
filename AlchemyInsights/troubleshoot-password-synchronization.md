---
title: Paroļu sinhronizēšanas problēmu novēršana
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
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664933"
---
# <a name="troubleshoot-password-synchronization"></a>Paroļu sinhronizēšanas problēmu novēršana

Lai novērstu paroļu sinhronizēšanas problēmas, vispirms izmantojiet šo AAD Connect problēmu novēršanas uzdevumu, lai noskaidrotu, kāpēc paroles netiek sinhronizētas. Lai sāktu, dodieties uz [Pārvaldīt tiešo sinhronizāciju](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Azure AD Connect serverī atveriet jaunu Windows PowerShell sesiju un atlasiet opciju **Palaist kā administratoram** .

2. Palaidiet Set-ExecutionPolicy RemoteSigned vai Set-ExecutionPolicy neierobežoti.

3. Startējiet Azure AD Connect vedni.

4. Dodieties uz lapu papildu **uzdevumi >** tālāk norādītās darbības  >  **Next**.

5. Atlasiet **palaist** , lai atvērtu PowerShell problēmu novēršanas izvēlni.

6. Atlasiet **paroļu sinhronizēšanas problēmu novēršana**.

    Šī problēma parasti ir tā, ka parole netiek sinhronizēta noteiktam lietotāja kontam.

    **Piezīmju** veikšana Paroļu sinhronizēšana neizdodas, ja pēdējā veiksmīgā paroļu sinhronizācija bija pirms kāda laika.

Papildu palīdzību par paroļu sinhronizācijas problēmu novēršanu skatiet rakstā [paroļu jaukšanas sinhronizācijas problēmu novēršana, izmantojot AZURE ad Connect sinhronizāciju](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).