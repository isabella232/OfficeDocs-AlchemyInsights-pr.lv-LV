---
title: SMTP autentifikācijas un problēmu novēršanas iespējošana
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 14f1454ad687b4d76cf419583b442685fa19b5a2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321760"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>SMTP autentifikācijas un problēmu novēršanas iespējošana

Ja vēlaties iespējot SMTP autentifikāciju pastkastei vai saņemat kļūdu "Klients nav autentificēts", "Autentifikācija nesekmīga" vai "SmtpClientAuthentication" ar kodu 5.7.57 vai 5.7.3 vai 5.7.139, kad mēģināt nosūtīt e-pasta ziņojumu, autentificējot ierīci vai lietojumprogrammu ar Microsoft 365, veiciet šīs trīs darbības, lai atrisinātu šo problēmu:

1. Atspējojiet [Azure drošības noklusējumus,](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) izslēdzot opciju **Iespējot drošības noklusējumus** uz **Nē.**

    A. Pierakstieties Azure portālā kā drošības administrators, nosacījum piekļuves administrators vai globālais administrators.<BR/>
    b. Pārlūkojot atrodiet Azure Active Directory > **rekvizīti.**<BR/>
    c. Atlasiet **Pārvaldīt drošības noklusējumus**.<BR/>
    d. Iestatiet **Iespējot drošības noklusējumus** **uz Nē**.<BR/>
    e. Atlasiet **Saglabāt**.

2. [Licencētajā pastkastē iespējojiet](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) klienta SMTP iesniegšanu.

    A. Izvēlnē Microsoft 365 administrēšanas centrs dodieties uz **Aktīvie lietotāji** un atlasiet lietotāju.<BR/>
    b. Dodieties uz cilni Pasts un sadaļā **E-pasta programmas** atlasiet Pārvaldīt **e-pasta programmas**.<BR/>
    d. **Pārliecinieties, vai ir atzīmēta** opcija Autentificēts SMTP (iespējots).<BR/>
    e. Atlasiet **Saglabāt izmaiņas**.<BR/>

3. [Atspējojiet daudzfaktors autentifikācijas (multi-Factor Authentication — MFA)](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) licencētajā pastkastē.

    A. Dodieties uz Microsoft 365 administrēšanas centrs un kreisajā navigācijas izvēlnē atlasiet Lietotāji  >  **Aktīvie lietotāji**.<BR/>
    b. Atlasiet **Daudzfaktors autentifikācija**.<BR/>
    c. Atlasiet lietotāju un atspējojiet **Daudzfaktors autentifikāciju**.<BR/>
