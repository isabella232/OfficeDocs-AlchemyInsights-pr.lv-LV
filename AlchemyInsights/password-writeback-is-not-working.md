---
title: Paroles rakstīšanas nedarbojas
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
ms.openlocfilehash: 679dea6d488cf74f51baee2b3b498dc64b95530e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324930"
---
# <a name="password-writeback-is-not-working"></a>Paroles rakstīšanas nedarbojas

**Man radušās problēmas ar paroles atraksta konfigurēšanu**

- Paroles rakstīšana ir premium līdzeklis.
- Pārliecinieties, vai izprotat licencēšanas prasības:
  - Jūsu organizācijā ir jābūt piešķirtai vismaz vienai licencei.
  - **Tikai mākonī pieejami** lietotāji — Office 365 (O365) maksas SKU vai Azure AD Basic
  - **Mākonis un/vai** lokālie lietotāji — Azure AD Premium P1 vai P2, Enterprise Mobility + Security (EMS) vai Secure Productive Enterprise (SPE)
    - Papildinformāciju par licencēšanas prasībām skatiet [rakstā Azure AD pašapkalpošanās paroles atiestatīšanas licencēšanas prasības.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Jums ir vismaz viens administratora konts un viens testa lietotāja konts ar vienu no atbilstošo licenci.
- Lai paroles rakstīšana darbotos, Savienošana Azure AD domēna kontrollera emulatoram ir jāpievieno primārā domēna kontrollera emulators. Varat konfigurēt Azure AD Savienošana primārā domēna kontrolleri, ar peles  labo pogu noklikšķinot uz Active Directory sinhronizācijas savienotāja rekvizītiem un pēc tam atlasot **konfigurēt direktorija nodalījumus**. Šajā sadaļā meklējiet domēna **kontrollera savienojuma iestatījumu** sadaļu un atzīmējiet izvēles rūtiņu ar nosaukumu **Tikai vēlamie domēna kontrolleri**.
    **Piezīme.** Ja vēlamais DC nav PDC emulators, Azure AD Savienošana joprojām sazināties ar PDC, lai rakstītu ar paroli.
- Paroles atiestatīšana ir konfigurēta un iespējota jūsu nomniekā. Papildinformāciju skatiet rakstā [Azure AD paroļu atiestatīšanas iespējošana lietotājiem.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)
- Pārliecinieties, vai administratora konts, kas tiek izmantots paroles rakstīšanas iespējošanai, ir mākoņa administratora konts (izveidots Azure AD, kas nav lokāli AD)
- Jums ir viens vai vairāku mežu AD lokāls izvietojums, kurā darbojas Windows Server 2008 R2, Windows Server 2012 vai Windows Server 2012 R2 ar instalētām jaunākajām servisa pakotnēm
- Ir instalēts rīks Azure AD Savienošana un esat sagatavojis savu AD vidi sinhronizēšanai mākonī. Pirms paroles rakstīšanas pārbaudes pārliecinieties, vai vispirms esat pabeidzis pilnu importēšanu un pilnu sinhronizāciju no AD un Azure AD azure AD ar Azure AD Savienošana.
- Lai uzzinātu vairāk, skatiet, kā veikt [pilnu sinhronizāciju un pilnu importēšanu Azure AD Savienošana](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Man ir problēma ar paroles atraksta savienojamību**

1. Lejupielādējiet un iespējojiet jaunāko [Azure AD versiju Savienošana](https://www.microsoft.com/download/details.aspx?id=47594)
2. Ugunsmūra konfigurācija: Azure AD Savienošana rīkam (1.1.443 un vairāk) būs nepieciešama **izejošā HTTPS** piekļuve, lai:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Atļaut dīkstāves savienojumiem saglabāties vismaz 2–3 minūtes

**Joprojām pastāv problēmas ar paroles atriti**

- Ja joprojām rodas problēmas, rīkā Azure AD Savienošana mēģiniet atspējot un atkārtoti iespējot paroles Savienošana pakalpojumu
- Papildinformāciju skatiet rakstā [Paroļu rakstīšanas atspējošana un atkārtota iespējošana](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
