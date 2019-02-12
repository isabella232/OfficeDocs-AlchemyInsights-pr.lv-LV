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
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: d346cf97fb2fd08a9132904517192d8728ffa941
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/12/2019
ms.locfileid: "29924703"
---
# <a name="troubleshoot-password-synchronization"></a>Problēmu novēršana darbā ar paroles sinhronizācija

Novērst problēmas, kur bez paroles tiek sinhronizēti ar Azure AD savienot versiju 1.1.614.0 vai jaunāka versija:
  
1. Atvērt jaunu Windows PowerShell sesijā Azure AD savienojumu servera opciju **Palaist kā administratoram** . 
    
2. Palaist **Set ExecutionPolicy RemoteSigned** vai **neierobežotu kopu ExecutionPolicy**. 
    
3. Startēt vedni Azure AD savienojumu.
    
4. Naviģējiet uz * papilduzdevumus * * lapu, izvēlieties * * novēršana * *, un noklikšķiniet uz **Next (tālāk**). 
    
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
  

