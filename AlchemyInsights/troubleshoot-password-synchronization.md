---
title: Problēmu novēršana paroļu sinhronizēšana
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732517"
---
# <a name="troubleshoot-password-synchronization"></a>Problēmu novēršana paroļu sinhronizēšana

Lai novērstu problēmas, ja nav paroļu sinhronizētas ar Azure AD Connect versiju 1.1.614.0 vai jaunāka versija:
  
1. Atveriet jaunu Windows PowerShell sesiju savā Azure AD Connect serverī, izmantojot opciju **Palaist kā administratoram** .

2. Palaidiet **Set-Executionpolicy RemoteSigned** vai **Set-Executionpolicy neierobežoti**.

3. Startējiet vedni Azure AD Connect.

4. Pārejiet uz **papildu uzdevumu** lapu, atlasiet **problēmu novēršana**un noklikšķiniet uz **Tālāk**.

5. Problēmu novēršanas lapā, noklikšķiniet uz Sākt, **lai sāktu problēmu novēršanas** izvēlni PowerShell.

6. Galvenajā izvēlnē atlasiet **problēmu novēršana paroļu sinhronizēšana**.

7. Apakšizvēlnē atlasiet **paroļu sinhronizēšana**nedarbojas vispār.

**Izprastu problēmu novēršanas uzdevuma rezultātus**
  
Problēmu novēršanas uzdevums veic šādas pārbaudes:
  
- Apstiprina, ka paroļu sinhronizēšana līdzeklis ir iespējots Azure AD nomnieka.

- Apstiprina, ka Azure AD Connect serveris nav sagatavošanas režīmā.

- Katram esošajam lokālā Active Directory savienotājs (kas atbilst esošo Active Directory mežā):

- 
  - Pārbauda, vai paroļu sinhronizēšana līdzeklis ir iespējots.

  - Meklē paroļu sinhronizēšana Periodisko kontrolziņojumu notikumus Windows lietojumprogrammu notikumu žurnālos.

  - Par katru Active Directory domēna lokālā Active Directory savienotājs:

  - Validē, ka domēns ir sasniedzams no Azure AD savienojumu servera.

  - Apstiprina, ka Active Directory domēna pakalpojumus (AD DS) kontiem, ko izmanto lokālā Active Directory savienotājs ir pareizs lietotājvārds, parole, un atļaujām, kas nepieciešamas paroļu sinhronizēšana.

Lai iegūtu palīdzību problēmu novēršana paroļu sinhronizēšana, skatiet [problēmu novēršana paroļu sinhronizēšana ar AZURE ad savienojumu sinhronizācija](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  