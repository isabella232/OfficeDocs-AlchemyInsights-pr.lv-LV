---
title: Paroļu sinhronizācijas problēmu novēršana
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387884"
---
# <a name="troubleshoot-password-synchronization"></a>Paroļu sinhronizācijas problēmu novēršana

Lai novērstu paroļu sinhronizēšanas problēmas, sāciet ar šo AAD savienojumu problēmu novēršanas uzdevumu, lai noteiktu, kāpēc paroles netiek sinhronizētas. Lai sāktu, dodieties uz [Pārvaldīt tiešo sinhronizāciju](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Azure AD savienojumu serverī atveriet jaunu Windows PowerShell sesiju un atlasiet opciju **Palaist kā** administratoram.

2. Palaidiet Set-ExecutionPolicy RemoteSigned vai Set-ExecutionPolicy neierobežots.

3. Azure AD savienojumu izveides vedņa startēšana.

4. Dodieties uz lapu Papildu uzdevumi > **Problēmu**  >  **novēršana Tālāk**.

5. Atlasiet **Palaist,** lai atvērtu PowerShell problēmu novēršanas izvēlni.

6. Atlasiet **Problēmu novēršana par paroļu sinhronizāciju**.

    Problēma parasti ir parole nav sinhronizēta konkrētu lietotāja kontu.

    **Piezīmes** Paroļu sinhronizēšana neizdodas, ja pēdējā veiksmīgā paroles sinhronizēšana bija pirms kāda laika.

Lai saņemtu papildu palīdzību paroļu sinhronizēšanas problēmu novēršanu, [skatiet rakstu Paroļu jaucējprogramma sinhronizēšanas problēmu novēršana ar Azure AD Connect sinhronizāciju](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).