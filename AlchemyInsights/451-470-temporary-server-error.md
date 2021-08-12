---
title: 451 4.7.0 Pagaidu servera kļūda. Lūdzu, vēlāk mēģiniet vēlreiz. PRX4
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2021
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "3000003"
- "12465"
ms.openlocfilehash: ce898981d053c8b5dc080ee83434bdacd7f02a636f0183293915bacdb48ba4ef
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812583"
---
# <a name="451-470-temporary-server-error-please-try-again-later-prx4"></a>451 4.7.0 Pagaidu servera kļūda. Lūdzu, vēlāk mēģiniet vēlreiz. PRX4

Sūtot e-pasta ziņojumu, izmantojot Smarthost "smtp.office365.com", var rasties problēma, izmantojot SMTP klienta iesniegšanas metodi, un tiek parādīta kļūda "451 4.7.0 pagaidu servera kļūda. Lūdzu, vēlāk mēģiniet vēlreiz. PRX4 galvenokārt ir pagaidu." 

Pārliecinieties, vai neizmantojat koplietojamu pastkasti SMTP klienta iesniegumiem, jo SMTP klienta iesniegšanas metodei ir nepieciešama licencēta pastkaste pasta sūtīšanai. Tomēr, ja neizmantojat koplietojamu pastkasti un problēma joprojām pastāv, pārbaudiet šādus iestatījumus:

1. Iespējot klienta SMTP iesniegumu licencētajā pastkastē, kas tiek izmantota, izpildot šo PowerShell komandu:

    ```Set-CASMailbox -Identity sean@contoso.com -SmtpClientAuthenticationDisabled $false```

    VAI

    1. Dodieties uz Microsoft 365 administrēšanas centrs > **Aktīvie** lietotāji un atlasiet lietotāju.
    1. Dodieties uz cilni Pasts un > **e-pasta** > atlasiet Pārvaldīt **e-pasta programmas**. 
    1. Pārliecinieties, **vai ir atzīmēts** iestatījums Autentificēts SMTP (iespējots).
    1. Atlasiet **Saglabāt izmaiņas**.
    
    Lai iespējotu SMTP autentifikāciju visai organizācijai, izpildiet šo komandu:

    `Set-TransportConfig -SmtpClientAuthenticationDisabled $true`
 
    **Piezīme.** Drošības apsvērumu dēļ ir ieteicams iespējot SMTP autentifikāciju tikai izmantotajām pastkastēm. Lietotāja līmeņa iestatījums ignorē organizācijas līmeņa iestatījumu.

2. Atspējojiet Azure drošības noklusējumus, izslēdzot Opciju **Iespējot drošības noklusējumus** uz **Nē:**

    1. Pierakstieties Azure portālā kā drošības administrators, nosacījum piekļuves administrators vai globālais administrators.
    1. Atrodiet visus Azure Active Directory >**  rekvizītus** un atlasiet **Pārvaldīt drošības noklusējumus**.
    1. Pārslēdziet **iestatījumu Iespējot drošības noklusējumus** uz **Nē**.
    1. Atlasiet **Saglabāt**.

3. Izmantotajā licencētajā pastkastē atspējojiet daudzpakāpju autentifikāciju (Multi Factor Authentication - MFA).

    1. Dodieties uz Microsoft 365 administrēšanas centrs un kreisajā navigācijas izvēlnē izvēlieties Lietotāji  >  **Aktīvie lietotāji.**
    1. Lapā **Aktīvie lietotāji** izvēlieties **Daudzfaktors autentifikācija**.
    1. Atlasiet lietotāju un atspējojiet **daudzfaktors autentifikāciju**.

