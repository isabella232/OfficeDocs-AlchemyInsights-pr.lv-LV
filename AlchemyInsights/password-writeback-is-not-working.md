---
title: Paroļu arī atpakaļrakstīšanas nedarbojas
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243515"
---
# <a name="password-writeback-is-not-working"></a>Paroļu arī atpakaļrakstīšanas nedarbojas

**Man rodas problēmas, konfigurējot paroļu arī atpakaļrakstīšanas**

- Paroļu arī atpakaļrakstīšanas ir Premium līdzeklis.
- Pārliecinieties, vai jums ir izpratne par licencēšanas prasībām:
  - Jums ir nepieciešama vismaz viena licence, kas piešķirta jūsu organizācijā
  - **Tikai mākoņi** — visi Office 365 (O365) apmaksātie SKU vai Azure AD Basic
  - **Mākoņa un/vai Lokālie lietotāji** — Azure AD Premium P1 vai P2, Enterprise Mobility + Security (EMS) vai Secure ražīgs uzņēmums (SPE)
    - Papildinformāciju par licencēšanas prasībām skatiet rakstā Azure AD pašapkalpošanās [paroles atiestatīšanas licencēšanas prasības](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Jums ir vismaz viens administratora konts un viens testa lietotāja konts ar vienu no attiecīgās licences.
- Lai strādātu ar paroļu arī atpakaļrakstīšanas, ir jāizveido savienojums ar Azure AD savienojumu ar primāro domēna kontrollera administratoru. Azure AD Connect varat konfigurēt, lai izmantotu primāro domēna kontrolleri, ar peles labo pogu noklikšķinot uz Active Directory sinhronizācijas savienotāja **rekvizītiem** un pēc tam atlasot **konfigurēt direktoriju nodalījumus**. Šeit meklējiet sadaļu **domēna kontrollera savienojuma iestatījumi** un atzīmējiet izvēles rūtiņu **izmantot tikai vēlamos domēna kontrollerus**.
  > [!NOTE]
  > Ja vēlamais DC nav PDC emulators, Azure AD Connect joprojām sasniedz PDC paroļu arī atpakaļrakstīšanas.
- Paroles atiestatīšana ir konfigurēta un iespējota jūsu nomniekā. Lai iegūtu papildinformāciju, skatiet rakstu [kā atļaut lietotājiem atiestatīt savas AZURE ad paroles](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).
- Pārliecinieties, vai administratora konts, kas tiek izmantots, lai iespējotu paroļu arī atpakaļrakstīšanas, ir mākoņa administratora konts (izveidots Azure AD nav lokālās reklāmas)
- Jums ir viena vai vairāku mežu reklāma lokālajā izvietojumā, kurā darbojas sistēma Windows Server 2008 R2, Windows Server 2012 vai Windows Server 2012 R2 ar pēdējām instalētajām servisa pakotnēm
- Jūs esat instalējis Azure AD Connect instrumentu un esat sagatavojis savu reklāmas vidi, lai sinhronizētu mākonī. Pirms paroļu arī atpakaļrakstīšanas pārbaudes vispirms pārliecinieties, vai esat pabeidzis pilnu importēšanu un pilnīgu sinhronizāciju no AD un Azure AD Azure AD Connect.
- Lai uzzinātu vairāk, skatiet rakstu kā veikt [pilno sinhronizāciju un pilnīgu importēšanu AZURE ad Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Man radās problēma ar paroļu arī atpakaļrakstīšanas savienojumu**

1. Jaunākās [AZURE ad Connect](https://www.microsoft.com/download/details.aspx?id=47594) versijas lejupielāde un iespējošana
2. Ugunsmūra konfigurācija: Azure AD Connect rīkam (1.1.443 un augstāk) vajadzēs **izejošo https** piekļuvi:
    - passwordreset.microsoftonline.com
    - servicebus. Windows. Networks
3. Atļaut saglabāt dīkstāvi vismaz 2-3 minūtes

**Joprojām pastāv problēmas ar paroļu arī atpakaļrakstīšanas**

- Ja joprojām rodas problēmas, mēģiniet atspējot un atkārtoti iespējot paroļu arī atpakaļrakstīšanas pakalpojumu Azure AD Connect rīkā
- Lai uzzinātu vairāk, skatiet rakstu kā [Atspējot un atkārtoti iespējot paroļu arī atpakaļrakstīšanas](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
