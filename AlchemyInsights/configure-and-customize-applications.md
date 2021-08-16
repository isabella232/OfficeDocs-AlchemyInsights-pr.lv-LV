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
ms.openlocfilehash: 3ce5b04469eb655c9d682f5830d9f906529aa40f706ee594b670708426d48769
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044995"
---
# <a name="configure-and-customize-applications"></a>Lietojumprogrammu konfigurēšana un pielāgošana

**Lietojumprogrammu konfigurēšana**

1. [Īsā pamācība: konfigurējiet](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) lietojumprogrammas rekvizītus Azure Active Directory (Azure AD) nomniekā, lai uzzinātu, kā konfigurēt dažus lietojumprogrammas rekvizītus.
2. Lai palīdzētu integrēt jūsu lietojumprogrammas Azure Active Directory, [](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) mēs esam izstrādājuši apmācību kolekciju, kurā ir izstrādāta konfigurēšana.
3. [Lietojumprogrammas starpniekservera lietojumprogrammas](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) konfigurēšana palīdz jums saprast, kā konfigurēt lietojumprogrammas starpniekservera lietojumprogrammu azure AD, lai atklātu lokālās lietojumprogrammas mākonī.
4. [Lejupielādējiet PingAccess](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)un konfigurējiet savu lietojumprogrammu: Izpildiet rakstā *Azure AD PingAccess* konfigurēšana sniegtos norādījumus, lai aizsargātu lietojumprogrammas, kas publicētas, izmantojot Microsoft Azure AD lietojumprogrammu starpniekserveri ping identitātes tīmekļa vietnē, un lejupielādējiet jaunāko PingAccess versiju.

**Nepareizi konfigurētas lietojumprogrammas (AADSTS650056) kļūdas**

1. Pārliecinieties, vai piekļūstat programmai no lietojumprogrammas īpašnieka nodrošinātās pierakstīšanās adreses. Pretējā gadījumā pierakstieties lietojumprogrammā, veicot standarta procesu. Vairākumā gadījumu tā automātiski tiek atrisināta dabiski. Ja tā nenotiek, šī ziņa var palīdzēt novērst problēmas un novērst problēmu.
2. **Ja jūsu organizācijai pieder programma** (kas nozīmē, ka pieteikuma reģistrācija ir jūsu organizācijā):
    - Mēs iesakām vismaz pievienot `User.Read` Microsoft Graph `openid` pilnvaroto atļauju. 
    - Pārliecinieties, vai lietojumprogrammai un visām tās atļaujām tiek piekrists. To var pārbaudīt, apskatot **lietojumprogrammas** reģistrācijas kolonnu Statuss **API atļauju ietvaros.**
    - Dažos scenārijos programma var būt trešā puse, tomēr tā var būt reģistrēta jūsu organizācijā. Pārbaudiet, vai šī lietojumprogramma ir norādīta jūsu programmu reģistrācijās (nevis Enterprise lietojumprogrammās).
    - Ja joprojām tiek rādīts šis kļūdas ziņojums. Pēc tam, iespējams, būs jāveido piekrišanas URL, kas aprakstīts **4. darbībā.**
3. **Ja jūsu organizācija nav lietojumprogrammas īpašnieks un izmanto to kā trešās puses lietojumprogrammu:**
    - Ja esat globālais/uzņēmuma administrators, vajadzētu būt redzamam piekrišanas ekrānam. Pārliecinieties, vai ir atzīmēta **izvēles rūtiņa "Piekrišana jūsu organizācijas vārdā".**
    - Ja neredzat piekrišanas ekrānu, izdzēsiet Enterprise lietojumprogrammu un mēģiniet vēlreiz.
    - Ja joprojām tiek rādīts šis kļūdas ziņojums. Pēc tam, iespējams, būs jāveido piekrišanas URL, kas aprakstīts **4. darbībā.**
4. **Manuāli izveidojiet** izmantojamo piekrišanas URL. Ja lietojumprogramma ir paredzēta, lai piekļūtu konkrētam resursam, iespējams, nevarēsit izmantot Piekrišanas pogas no Azure portāla, jums būs manuāli jāģenerē savs piekrišanas VIETRĀDIs URL un jāizmanto šis.
    - Jums būs nepieciešams iegūt `{App-Id}` `{App-Uri-Id}` lietojumprogrammas īpašnieku un tā īpašnieku. `{Tenant-Id}` būs jūsu nomnieka identifikators. Tas būs vai nu `yourdomain.onmicrosoft.com` jūsu direktorija ID.
    - Ja lietojumprogrammai tiek piekļūts pats resursam, šī lietojumprogramma `{App-Id}` `{App-Uri-Id}` būs tā pati.
5. Papildinformāciju skatiet [rakstā Problēmas ar pierakstīšanos SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)vienotās pierakstīšanās konfigurētās programmās.

**Lietojumprogrammu pielāgošana**

- [Zīmola pievienošana](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) savas organizācijas Azure Active Directory pierakstīšanās lapā — izmantojiet savas organizācijas logotipu un pielāgotas krāsu shēmas, lai nodrošinātu konsekventu izskatu un darbību jūsu Azure Active Directory (Azure AD) pierakstīšanās lapās.
- [Pievienojiet savu pielāgoto domēna nosaukumu, izmantojot Azure Active Directory portālu](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) – Katram jaunajam Azure AD nomniekam ir sākotnējais domēna nosaukums. Sākotnējo domēna nosaukumu nevar mainīt vai izdzēst, taču varat pievienot savas organizācijas nosaukumus. Pievienojot pielāgotus domēnu nosaukumus, varat izveidot lietotājvārdus, kas ir pazīstami jūsu lietotājiem.
