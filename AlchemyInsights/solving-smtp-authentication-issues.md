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
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077658"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>SMTP autentifikācijas un problēmu novēršanas iespējošana

Ja vēlaties iespējot SMTP autentifikāciju pastkastei vai saņemat kļūdu "Klients nav autentificēts", "Autentifikācija nesekmīga" vai "SmtpClientAuthentication" ar kodu 5.7.57 vai 5.7.3 vai 5.7.139, kad mēģināt nosūtīt e-pasta ziņojumu, autentificējot ierīci vai lietojumprogrammu ar Microsoft 365, veiciet šīs trīs darbības, lai novērstu šo problēmu:

1. Atspējojiet [Azure drošības noklusējumus,](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) izslēdzot opciju **Iespējot drošības noklusējumus** uz **Nē**.

    a. Pierakstieties Azure portālā kā drošības administrators, nosacījum piekļuves administrators vai globālais administrators.<BR/>
    b. Pārlūkojot atrodiet Azure Active Directory > **rekvizīti.**<BR/>
    c. Atlasiet **Pārvaldīt drošības noklusējumus**.<BR/>
    d. Iestatiet **Iespējot drošības noklusējumus** **uz Nē**.<BR/>
    e. Atlasiet **Saglabāt**.

2. [Licencētajā pastkastē iespējojiet](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) klienta SMTP iesniegšanu.

    a. Izvēlnē Microsoft 365 administrēšanas centrs dodieties **uz Aktīvie** lietotāji un atlasiet lietotāju.<BR/>
    b. Dodieties uz cilni Pasts un sadaļā **E-pasta programmas** atlasiet Pārvaldīt **e-pasta programmas**.<BR/>
    d. **Pārliecinieties, vai ir atzīmēta** opcija Autentificēts SMTP (iespējots).<BR/>
    e. Atlasiet **Saglabāt izmaiņas**.<BR/>

3. [Atspējojiet daudzfaktors autentifikācijas (multi-Factor Authentication — MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) licencētajā pastkastē.

    a. Dodieties uz Microsoft 365 administrēšanas centrs un kreisajā navigācijas izvēlnē **atlasiet** Lietotāji  >  **Aktīvie lietotāji**.<BR/>
    b. Atlasiet **Daudzfaktors autentifikācija**.<BR/>
    c. Atlasiet lietotāju un atspējojiet **Daudzfaktors autentifikāciju**.<BR/>
