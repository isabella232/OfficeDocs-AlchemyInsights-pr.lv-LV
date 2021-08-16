---
title: Vietņu atklāšanas iespēja
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: 4653fdef7e9226f05809d56e9a445cd1da35b0578c088bea72252a281d4527d2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030765"
---
# <a name="do-site-discovery"></a>Vietņu atklāšanas iespēja

Ja jūsu organizācija joprojām izmanto mantotas tīmekļa lietojumprogrammas un plāno izmantot Internet Explorer režīmu (ko dara lielākā daļa klientu), ir jāveic papildu vietņu atklāšana.

**Jūs jau esat izvietojis vecāku programmas Microsoft Edge**

Ja jau esat konfigurējis uzņēmuma vietņu sarakstu darbam ar mantoto Microsoft Edge, vietņu atklāšana ir gandrīz pabeigta. Viena lieta, kas, iespējams, būs jāveic, ir neitrālu vietņu pievienošana.

Neitrālas vietnes parasti ir vietnes, kas nodrošina vienoto pierakstīšanās (single sign-on — SSO). Ja no neitrālas vietnes Microsoft Edge vēlaties turpināt izmantot Microsoft Edge autentificēšanu. Ja dodaties uz neitrālu vietni Internet Explorer režīmā, tad, lai autentificētu, vēlaties palikt Internet Explorer režīmā.

Identificējiet SSO vai citas neitrālas vietnes, ko izmantojat, un pievienojiet tās uzņēmuma vietņu sarakstam.

**Internet Explorer ir jūsu noklusējuma pārlūkprogramma**

Ja tagad izmantojat tikai pārlūkprogrammu Internet Explorer, iespējams, nezināt, kuras vietnes ir jauninātas uz moderniem tīmekļa standartiem un kurām joprojām ir nepieciešama programma Internet Explorer. Šīs vietnes vēlēsities atrast un pievienot uzņēmuma vietņu sarakstam, lai šajās vietnēs varētu izmantot tikai Internet Explorer režīmu.

> [!NOTE]
> [Uzņēmuma vietnes atklāšana](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) atrod vietnes, kurām var būt nepieciešams Internet Explorer režīms. Tas var apkopot datus datoros, kuros ir pārlūkprogramma Windows Internet Explorer 8 līdz Internet Explorer 11 Windows 10, Windows 8.1 vai Windows 7.

**Datu analīze**

Kad esat apkopojis vietnes datus, ir ieteicams veikt tālāk norādītās četras darbības, lai analizētu datus.
1. Kārtojiet datus pēc domēna un pēc tam pēc vietrāža URL.
2. Definējiet programmas robežas, lai konfigurētu Internet Explorer režīmu. Jūs vēlaties iekļaut visas vietnes un tīmekļa vadīklas, kas definē programmu, bet nevēlaties iekļaut papildu vietnes un vadīklas. Dažas vietnes var būt tik *https://contoso.com/app1* vienkāršas, cik vien citas var prasīt vairāku vietņu un lapu definēšanu.
3. Pārbaudiet programmu, lai pārliecinātos, vai tā nedarbojas iebūvēti. Daudzās vietnēs tiek piedāvāts moderns saturs, ja tās konstatē mūsdienīgu pārlūkprogrammu un piedāvā mantoto saturu tikai tad, ja tās konstatē Internet Explorer.
4. Ja neizdodas veikt testēšanu, pievienojiet lietojumprogrammu savam uzņēmuma vietņu sarakstam.

> [!NOTE]
> Ieteicamā prakse ir grupēt visas vietnes, kas veido lietojumprogrammu. Šādi, jauninot programmu, ir vieglāk noņemt visu vietni no Internet Explorer režīma un sākt izmantot modernu šīs lietojumprogrammas pārlūkprogrammu.

Kad esat beidzis vietņu atklāšanu un analizējis datus, varat sākt apskatīt savu kanāla stratēģiju.

