---
title: Lietojumprogrammu konfigurēšana un pielāgošana
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
- "9004334"
- "7733"
ms.openlocfilehash: 30127beda85dd9824f7e3a7a4744d109e7ea874b
ms.sourcegitcommit: aeb15e206865f61ff61a1e55c407e34eaa89b6d1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063658"
---
# <a name="configure-and-customize-applications"></a>Lietojumprogrammu konfigurēšana un pielāgošana

**Lietojumprogrammu konfigurēšana**

1. [Quickstart: lietojumprogrammas rekvizītu konfigurēšana savā Azure Active Directory (AZURE AD) nomniekā](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) ir parādīts, kā konfigurēt dažus lietojumprogrammas rekvizītus.
2. Lai palīdzētu integrēt lietojumprogrammas, izmantojot pakalpojumu Azure Active Directory, mēs esam izveidojuši [apmācību apkopojumu](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) , kas palīdzēs jums veikt konfigurēšanu.
3. [Lietojumprogrammas starpniekservera lietojumprogrammas konfigurēšana](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) palīdz saprast, kā konfigurēt lietojumprogrammas starpniekservera lietojumprogrammu Azure AD, lai lokālās lietojumprogrammas atklātu mākonī.
4. [Lejupielādējiet PingAccess un konfigurējiet lietojumprogrammu](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application): izpildiet norādījumus rakstā *PINGACCESS konfigurēšana Azure AD, lai aizsargātu lietojumprogrammas* , kas publicētas, izmantojot Microsoft Azure AD lietojumprogrammas starpniekserveri, ping identitātes vietnē un lejupielādējot jaunāko PingAccess versiju.

**Nepareizi konfigurētas lietojumprogrammu (AADSTS650056) kļūdas**

1. Pārliecinieties, vai piekļūstat lietojumprogrammai no lietojumprogrammas īpašnieka nodrošinātās pierakstīšanās adreses. Pretējā gadījumā pierakstieties lietojumprogrammā, izmantojot parasto procesu. Vairumā gadījumu tas tiks automātiski atrisināts dabiski. Ja tā nav, šī ziņa var palīdzēt novērst un atrisināt to.
2. **Ja jūsu organizācijai pieder lietojumprogramma** (tas nozīmē, ka lietojumprogrammas reģistrācija ir jūsu organizācijā):
    - Vismaz mēs iesakām `User.Read` `openid` Pievienot vai pilnvaroto atļauju no **Microsoft Graph** .
    - Nodrošiniet, lai lietojumprogramma un visas tās atļaujas tiktu sūtītas. Varat to pārbaudīt, aplūkojot **API atļauju** lietojumprogrammas reģistrācijas kolonnas **statusu** .
    - Dažos scenārijos lietojumprogramma var būt trešās puses, taču tā var būt reģistrēta jūsu organizācijā. Apstipriniet, vai šī lietojumprogramma ir norādīta jūsu lietojumprogrammu reģistrācijās (nevis uzņēmuma lietojumprogrammās).
    - Ja joprojām tiek rādīts šis kļūdas ziņojums. Pēc tam jums, iespējams, būs jāveido 4. **darbībā** aprakstītais piekrišanas vietrādis URL.
3. **Ja jūsu organizācija nav lietojumprogrammas īpašnieks un izmanto to kā trešo personu lietojumprogrammu**:
    - Ja esat globālais/uzņēmuma administrators, jums ir jābūt redzamam piekrišanas ekrānam. Pārliecinieties, vai ir atzīmēta izvēles rūtiņa **"piekrišana organizācijas vārdā"**.
    - Ja neredzat ekrānu piekrišana, izdzēsiet uzņēmuma lietojumprogrammu un mēģiniet vēlreiz.
    - Ja joprojām tiek rādīts šis kļūdas ziņojums. Pēc tam jums, iespējams, būs jāveido 4. **darbībā** aprakstītais piekrišanas vietrādis URL.
4. **Manuāli izveidot piekrišanas vietrādi URL, kas jāizmanto**: ja lietojumprogramma ir izstrādāta, lai piekļūtu noteiktam resursam, iespējams, nevarēsit izmantot pogas apstiprinājums no Azure portāla, jums ir manuāli jāģenerē sava piekrišana un jāizmanto šis.
    - Jums ir jāiegūst `{App-Id}` un `{App-Uri-Id}` no lietojumprogrammas īpašnieka. `{Tenant-Id}` būs jūsu nomnieka identifikators. Šī darbība būs `yourdomain.onmicrosoft.com` vai jūsu DIREKTORIJA ID.
    - Ja lietojumprogramma piekļūst resursam, tad `{App-Id}` un `{App-Uri-Id}` būs tas pats.
5. Papildinformāciju skatiet rakstā problēmas, [Pierakstoties SAML vienotās pierakstīšanās programmas](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application).

**Lietojumprogrammu pielāgošana**

- [Pievienojiet zīmolu savas organizācijas Azure Active Directory pierakstīšanās lapā](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) — Izmantojiet savas organizācijas logotipu un pielāgotas krāsu shēmas, lai nodrošinātu konsekventu izskatu ar savu Azure Active Directory (Azure AD) pierakstīšanās lapu.
- [Pievienojiet savu pielāgoto domēna nosaukumu, izmantojot Azure Active Directory portālu](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) — katram jaunajam Azure AD nomniekam ir sākotnējais domēna nosaukums. Jūs nevarat mainīt vai izdzēst sākotnējo domēna nosaukumu, bet varat pievienot savas organizācijas vārdus. Pievienojot pielāgotus domēnu nosaukumus, varat izveidot lietotājiem pazīstamus lietotāju vārdus.
