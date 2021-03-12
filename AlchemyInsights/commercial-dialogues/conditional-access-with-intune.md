---
title: Ierobežotas piekļuves izmantošana ar Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746031"
---
# <a name="using-conditional-access-with-intune"></a>Ierobežotas piekļuves izmantošana ar Intune

Ierobežotas piekļuves izmantošanai ar Intune ir jāveic 3 darbības:

- [Izveidojiet atbilstības politiku, lai definētu iestatījumus, kas jāizpilda, pirms ierīce tiek uzskatīta par atbilstošu. Piemēram, ierīcei ir jābūt vismaz 6 ciparu spraudīti, pirms tā tiek uzskatīta par atbilstošu.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Izveidojiet nosacījuma piekļuves politiku, kas nosaka, kādi resursi tiek aizsargāti, un kādi nosacījumi ir jāievēro, lai piekļūtu šiem resursiem. Piemēram, ierīcei ir jābūt savietojamai, pirms piekļūstat korporatīvajam e-pastam.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Nodrošināt, lai atbilstības politikas un ierobežotas piekļuves politikas būtu paredzētas vajadzīgajām lietotāju grupām. Tam var būt nepieciešama noteiktu lietotāju grupu izveide Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Papildinformācija...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
