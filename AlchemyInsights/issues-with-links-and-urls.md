---
title: Problēmas ar saitēm un vietrāžiem URL
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: 1387d7e0cdf2e730b2812f3970181d2bf889d44b1faab9a351911840909defb5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054805"
---
# <a name="issues-with-links-and-urls"></a>Problēmas ar saitēm un vietrāžiem URL

Novirzīšanas URI/atbilžu vietrāži URL (abas izteiksmes ir apmaināmas) ir vietrāži URL, ko izmanto Microsoft identitātes platforma, lai atgrieztu lietojumprogrammu pieprasītās pilnvaras. Informāciju par šiem vietrāžiem URL skatiet šajos rakstos:

- [Autentifikācijas plūsmas un lietojumprogrammu scenāriji](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) — informācija par novirzīšanas URI **programmas reģistrācijas** lapā katram scenārijam.
- [Novirzīšanas URI/atbildes vietrāža URL ierobežojumi](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Es nezinu, kā reģistrēt pareizo novirzīšanas URI/atbildes vietrādi URL manai lietojumprogrammai**

Ja pierakstāties ar izstrādājamo lietojumprogrammu un pierakstīšanās dialoglodziņā tiek parādīts **AADSTS50011: pieprasījumā norādītais atbildes vietrādis URL neatbilst lietojumprogrammai <your app ID>** konfigurētajiem atbilžu vietrāžiem URL, jums ir jāpievieno lietojumprogrammas reģistrācijai novirzīšanas URI, kuru jūsu kods izmantoja pilnvaras pieprasījumā Microsoft identitātes platformai.

Lai pievienotu atbildes vietrādi URL, Azure portāla **lietojumprogrammu reģistrācijas** lapā dodieties uz cilni **Autentifikācija** un pievienojiet ierakstu sadaļā **Novirzīšanas URI**. Ievadāmā vērtība ir atkarīga no izstrādājamās lietojumprogrammas tipa, kā aprakstīts tālāk:

- Vienas lapas lietojumprogrammām un tīmekļa lietojumprogrammām atbildes vietrādis URL ir vietrādis URL jūsu lietojumprogrammā. Skatiet rakstu [Vienas lapas lietojumprogrammas reģistrācija](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) vai [Tīmekļa programmas reģistrācija, izmantojot Azure portālu](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- Datora programmām ievadāmā vērtība ir atkarīga no:
    - platformas (MacOS atšķiras no Windows vai Linux)
    - veida, kā iegūstat pilnvaru (interaktīvi, ar ierīces kodu plūsmu, ar integrēto Windows autentifikāciju [IWA] vai ar lietotājvārdu/paroli).
    Detalizētu informāciju skatiet sadaļā [Datora programmas — Programmu reģistrācija — Novirzīšanas URI](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- Mobilajām lietojumprogrammām novirzīšanas URI ir atkarīgs no:
    - platformas (iOS/Android/UWP)
    - informācijas, kas izmantota jūsu programmas izstrādei, piemēram, komplekta ID operētājsistēmā iOS, un pakotnes nosaukuma un paraksta jaukšanas operētājsistēmā Android. Jums palīdzēs Azure portāla programmu reģistrācija. Detalizētu informāciju skatiet rakstā [Platformas konfigurācija un novirzīšanas URI](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> Tīmekļa API un dažiem nemanāmiem pilnvaru iegūšanas veidiem (IWA un lietotājvārds/parole) nav nepieciešams novirzīšanas URI.

**Esmu izvietojis savu tīmekļa lietojumprogrammu, un, testējot izvietoto programmu, tiek parādīts atbildes vietrāža URL neatbilstības ziņojums**

Pievienojiet novirzīšanas URI visām atrašanās vietām, kurās izvietojat savu tīmekļa lietojumprogrammu. Papildinformāciju skatiet rakstā [Tīmekļa programmas reģistrācija, izmantojot Azure portālu](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> Pievienojiet novirzīšanas URI atrašanās vietai uzreiz pēc tam, kad esat izvietojis lietojumprogrammu šajā atrašanās vietā.

**Nevaru reģistrēt pietiekami daudz atbilžu vietrāžu URL**

Jūs esat ISV, un jums ir viens vai vairāki novirzīšanas URI katram jūsu klientam. Jūs vēlaties migrēt no ADAL/Azure AD v1.0 uz MSAL/Microsoft identitātes platformu un esat sasniedzis [maksimālo novirzīšanas URI skaitu](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Lai šo problēmu atrisinātu, [pievienojiet novirzīšanas URI uz pakalpojumu identitātēm](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals), kas atbilst katram jūsu klientam.
