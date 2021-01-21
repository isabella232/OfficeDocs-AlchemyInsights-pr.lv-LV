---
title: Marķierierīces ilguma konfigurēšana un pagarināšana
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917004"
---
# <a name="configure-and-extend-token-lifetimes"></a>Marķierierīces ilguma konfigurēšana un pagarināšana

Varat norādīt, kāda ir Access, SAML vai ID pilnvara, ko izsniedz Microsoft Identity Platform. Varat iestatīt token mūžus visās programmās savā organizācijā, vairāku nomnieku (vairāku organizāciju) lietojumprogrammai vai konkrētam pakalpojumu pilnvarotājam jūsu organizācijā. Lai iegūtu papildinformāciju, izlasiet [konfigurējamas marķierierīces ilgumus](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

Piemēram, izlasiet [piemērus par to, kā konfigurēt marķierierīces ilgumu](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).

Lai uzzinātu, kā konfigurēt marķiera mūžu un saderību Azure Active Directory B2C (Azure AD B2C), skatiet rakstu [tokens konfigurēšana Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).

Rakstā [sesijas darbības konfigurēšana Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) apraksta vienotās pierakstīšanās (SSO) metodēs, ko izmanto AZURE ad B2C, un palīdz izvēlēties piemērotāko SSO metodi, konfigurējot politiku.

**Cik ilgi žetoni ir pēdējie? Cik ilgi tie ir derīgi?**

Token kalpošanas ilgums ir 1 stunda un sesijas ilgums ir 24 stundas. Tas nozīmē, ka, ja pieprasījumi nav veikti 24 stundās, jums ir atkārtoti jāpiesakās, lai tiktu pieprasīta jauna pilnvara.

> [!NOTE]
> Pēc 30. maija 2020 neviens jaunais nomnieks nevarēs izmantot konfigurējamu marķierierīces kalpošanas ilgumu, lai konfigurētu sesijas un atsvaidzināšanas marķierus. Novecošana notiks vairāku mēnešu laikā pēc tam, kas nozīmē, ka mēs pārstām ievērot pašreizējo sesiju un atsvaidzināt marķierus. Jūs joprojām varat konfigurēt piekļuves pilnvaru ilgumu pēc izslēgšanas.






