---
title: Lietotājs saņem kļūdu AADSTS7000112 Yammer ir atspējota
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198055"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a>Lietotājs saņem kļūdu AADSTS7000112 Yammer ir atspējota

Ja saņemat kļūdas ziņojumu "AADSTS7000112: lietojumprogramma '00000005-0000-0ff1-ce00-0000000000"(Yammer) ir atspējota", rodas problēma ar pakalpojuma vadītāju Azure AD. Administrators, iespējams, ir atspējojis pakalpojuma vadītāju, lai bloķētu piekļuvi Yammer.

Pakalpojuma vadītāja atspējošana nav ieteicama un var radīt papildu problēmas. Lai iegūtu papildinformāciju par atbalstīto pieeju, lai bloķētu lietotāju piekļuvi Yammer, [skatiet Yammer piekļuves izslēgšana Microsoft 365 lietotājiem](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).  

Lai novērstu šo problēmu Azure portālā un atjaunot lietotāja piekļuvi Yammer:

1.  Atveriet Azure Active Directory lapu un atlasiet **uzņēmuma lietojumprogrammas** **zem Pārvaldīt** kreisajā navigācijas rūtī.
3.  Meklēšanas **lodziņā ierakstiet Office 365 Yammer** un atlasiet lietojumprogrammas nosaukumu, lai atvērtu iestatījumus.
4.  Kreisajā **navigācijas** **rūtī atlasiet** Rekvizīti zem Pārvaldīt.
5.  Vai iestatīt vērtību **Yes** **Iespējots, lai lietotāji varētu pierakstīties?** **Save**
6.  Vēlreiz pierakstieties pakalpojumā Yammer. Iespējams, būs jānotīra sīkfaili.

Vai arī palaidiet PowerShell komandas, lai iestatītu vērtību. Lai iegūtu papildinformāciju, [skatiet "Atvainojiet, bet mums ir problēmas ar pierakstīšanos"kļūda, noklikšķinot uz Yammer mozaīkas Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365). 