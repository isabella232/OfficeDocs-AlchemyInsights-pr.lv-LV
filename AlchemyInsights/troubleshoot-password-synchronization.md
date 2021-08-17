---
title: Paroļu sinhronizācijas problēmu novēršana
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
ms.openlocfilehash: cb782c0d1dc396ee7a9f016afb9629a2cdee93d52f5408b7a73e576e783ebc0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105762"
---
# <a name="troubleshoot-password-synchronization"></a>Paroļu sinhronizācijas problēmu novēršana

Lai novērstu paroles sinhronizācijas problēmas, vispirms izmantojiet šo AAD Savienošana problēmu novēršanas uzdevumu, lai noteiktu, kāpēc netiek sinhronizētas paroles. Lai sāktu, dodieties uz [Tiešās sinhronizācijas pārvaldība.](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)  

1. Atveriet jaunu Windows PowerShell sesiju savā Azure AD Savienošana serverī un atlasiet **opciju Palaist kā administratoram.**

2. Palaidiet Set-ExecutionPolicy RemoteSigned vai Set-ExecutionPolicy Neierobežota.

3. Startējiet Azure AD Savienošana vedni.

4. Dodieties uz lapu Papildu uzdevumi un >  >  **Tālāk.**

5. Atlasiet **Palaist,** lai atvērtu PowerShell problēmu novēršanas izvēlni.

6. Atlasiet **Paroles sinhronizācijas problēmu novēršana**.

    Problēma parasti ir tā, ka konkrētam lietotāja kontam parole netiek sinhronizēta.

    **Piezīmes** Paroļu sinhronizācija neizdodas, ja pēdējā sekmīgā paroļu sinhronizācija bija veikta pirms kāda laika.

Papildu palīdzību paroļu sinhronizācijas problēmu novēršanai skatiet [rakstā Paroles jaukšanas sinhronizācijas problēmu novēršana, izmantojot Azure AD Savienošana sinhronizāciju.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)