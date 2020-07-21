---
title: Dzēst bāreņlietotāju no lokālā servera
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198181"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>Dzēst bāreņlietotāju no lokālā servera

Lai noņemtu savrupās lietotājs, rīkojieties šādi:

1. Vaibst direktorija sinhronizāciju, izpildot [norādījumus kas ir hibrīds identitāti ar Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).

2. Lai pārbaudītu direktoriju sinhronizāciju, skatiet [rakstu Kas ir hibrīda identitāte ar Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).

3. Ja sinhronizācija darbojas pareizi, bet Active Directory objektu dzēšana nav izplatīt Azure AD, manuāli noņemt savrupās objektu, izmantojot kādu no šīm Azure Active Directory modulis Windows PowerShell cmdlet:

    Noņemt MsolContact  
    Noņemt MsolGroup  
    Noņemt MsolUser

    Piemēram, lai noņemtu savrupās lietotāja ID john.smith@contoso.com, kas sākotnēji izveidots, izmantojot direktoriju sinhronizāciju, palaidiet cmdlet:

    Remove-MsolUser -UserPrincipal John.Smith@Contoso.comName Remove-MsolUser-UserPrincipalName