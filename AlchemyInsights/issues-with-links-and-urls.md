---
title: Problēmas ar saitēm un vietrāžiem URL
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: 24885d873d6471a72ae66581ad1ceb0a19b664f7
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974468"
---
# <a name="issues-with-links-and-urls"></a>Problēmas ar saitēm un vietrāžiem URL

Novirzīt URI/atbildes vietrāžus URL (abas izteiksmes ir savstarpēji aizvietojamas) ir vietrāži URL, ko izmanto Microsoft Identity Platform, lai atgrieztu lietojumprogrammas, kas pieprasītas. Informāciju par šiem vietrāžiem URL skatiet šajos rakstos:

- [Autentifikācijas plūsmas un lietojumprogrammas scenāriji](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) — informācija par novirzīšanas URI **lietojumprogrammas reģistrācijas** lapā katram scenārijam.
- [URI/atbildes URL novirzīšanas ierobežojumi](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Es nezinu, kā reģistrēt pareizo savas lietojumprogrammas Pārvirzīšanas URI/atbildes vietrādi URL**

Kad pierakstāties ar lietojumprogrammu, ko veidojat, ja pierakstīšanās dialogs parāda **AADSTS50011: pieprasījumā norādītais atbildes vietrādis URL neatbilst programmā <your app ID> konfigurētajiem atbilžu vietrāžiem URL**, jums ir jāpievieno lietojumprogrammas reģistrācija, kas norāda, ka jūsu kods, ko izmanto marķierierīces pieprasījumā, norāda uz Microsoft identitātes platformu.

Lai pievienotu atbildes vietrādi URL, Azure portālā atveriet  lapu **lietojumprogrammas reģistrācija** un pievienojiet ierakstu sadaļā **novirzīšanas URI** . Pārvirzīšanas URI ir ierakstīts (tīmeklī vai mobilajā datorā). Vērtība, kas jāievada, ir atkarīga no veidojamās lietojumprogrammas tipa, kā aprakstīts tālāk.

- Lai iegūtu atsevišķas lapas lietojumprogrammas un tīmekļa lietojumprogrammas, atbildes vietrādis URL ir vietrādis URL savā lietojumprogrammā. Skatīt [vienas lapas lietojumprogrammas reģistrāciju](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) vai [reģistrēt tīmekļa lietojumprogrammas programmu, izmantojot Azure Portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- Datora programmu gadījumā nepieciešamā vērtība jāizvēlas atkarībā no tā, vai:
    - platforma (MacOS atšķiras no Windows vai Linux)
    - veids, kādā jūs iegūstat pilnvarojumu (interaktīvi, ar ierīces koda plūsmu, ar integrētu Windows autentifikāciju [IWA] vai ar lietotājvārdu/paroli).
    Detalizētu informāciju skatiet rakstā [datora lietojumprogrammas — lietojumprogrammu reģistrācija — novirzīšanas URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- Mobilajām lietojumprogrammām novirzīšanas URI ir atkarīgs no:
    - platforma (iOS/Android/UWP)
    - informāciju, kas tiek izmantota lietojumprogrammas izveidei, piemēram, paketes ID iOS ierīcē, un pakotnes nosaukumu un paraksta hash Android ierīcē Azure Portal lietojumprogrammu Reģistrācija palīdzēs jums. Detalizētu informāciju skatiet rakstā [platformas konfigurēšana un URI novirzīšana](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> Tīmekļa API un dažiem slēptajiem veidiem, kā iegūt marķierus (IWA un username/password), nav nepieciešams novirzīt URI.

**Esmu izvietojis savu tīmekļa lietojumprogrammu, un, testējot izcelto lietojumprogrammu, tiek parādīts ziņojums par atbildes vietrādi URL neatbilstību**

Pievienojiet Pārvirzīšanas URI visām atrašanās vietām, kurās tiek izvietota tīmekļa lietojumprogramma. Papildinformāciju skatiet rakstā [tīmekļa lietojumprogrammas lietojumprogrammas reģistrēšana, izmantojot Azure Portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> Pievienojiet novirzīšanas URI atrašanās vietai tūlīt pēc tam, kad esat izvietojis lietojumprogrammu šajā atrašanās vietā.

**Nevaru reģistrēt pietiekami daudz atbildes URL**

Jūs esat ISV un jums ir viens vai vairāki novirzīšanas URI visiem klientiem. Jūs vēlaties migrēt no ADAL/Azure AD v 1.0 uz MSAL/Microsoft identitātes platformu, un jūs nosita [maksimālo Pārvirzīšanas URI skaitu](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Lai atrisinātu šo problēmu, [pievienojiet novirzīt URI pakalpojumu principāliem](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) , kas atbilst katram jūsu klientiem.
