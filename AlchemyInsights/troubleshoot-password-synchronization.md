---
title: Problēmu novēršana darbā ar paroles sinhronizācija
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 165e0ff4b2136b727450946d2c47756ebee7d393
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353112"
---
# <a name="troubleshoot-password-synchronization"></a>Problēmu novēršana darbā ar paroles sinhronizācija

Novērst problēmas, kur bez paroles tiek sinhronizēti ar Azure AD savienot versiju 1.1.614.0 vai jaunāka versija:
  
1. Atvērt jaunu Windows PowerShell sesijā Azure AD savienojumu servera opciju **Palaist kā administratoram** .

2. Palaist **Set ExecutionPolicy RemoteSigned** vai **neierobežotu kopu ExecutionPolicy**.

3. Startēt vedni Azure AD savienojumu.

4. Naviģējiet uz lapu **Papildu uzdevumus** , atlasiet **problēmu novēršana**un noklikšķiniet uz **Tālāk**.

5. Problēmu novēršana lapā noklikšķiniet uz **Sākt startēt problēmrisināšanas** menu PowerShell.

6. Galvenajā izvēlnē izvēlieties **Paroli sinhronizācijas problēmu novēršana**.

7. Apakšizvēlnes, izvēlieties **Paroles sinhronizācija nedarbojas vispār**.

**Izprast problēmu novēršanas uzdevumu rezultāti**
  
Problēmu novēršanas uzdevumu veic šādas pārbaudes:
  
- Apstiprina, ka parole sinhronizācijas līdzeklis ir iespējots debeszils AD īrnieks.

- Apstiprina, ka Azure AD savienojumu servera nav inscenējums režīmā.

- Par katru esošo lokālā Active Directory savienotāju (kas atbilst esošās Active Directory mežā):

- 
  - Apstiprina, ka parole sinhronizācijas līdzeklis ir iespējots.

  - Meklē paroles sinhronizācija sirdsdarbība notikumi Windows programmu notikumu žurnālos.

  - Katra domēna Active Directory sadaļā lokālā Active Directory savienotāju:

  - Apstiprina, ka domēns ir sasniedzams no Azure AD savienojumu servera.

  - Apstiprina, ka Active Directory domēna pakalpojumus (AD DS) kontus izmanto lokālā Active Directory savienotājs ir pareizais lietotājvārds, parole un atļauju parole sinhronizācijai nepieciešamos.

Papildu palīdzību problēmu novēršana sinhronizācijas paroli, skatiet [novēršana paroles sinhronizācija ar Azure AD pievienot sinhronizācijas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  