---
title: Veikt vietnes atklāšanu
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
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693484"
---
# <a name="do-site-discovery"></a>Veikt vietnes atklāšanu

Ja jūsu organizācijā joprojām tiek izmantotas mantotās tīmekļa lietojumprogrammas un plāni, lai izmantotu Internet Explorer režīmu (ko lielākā daļa klientu), jums jāveic papildu vietņu noteikšana.

**Jūs jau esat izvietojis vecāku Microsoft Edge versiju**

Ja jau esat konfigurējis savu uzņēmuma vietnes sarakstu, lai strādātu ar Microsoft Edge mantoto versiju, pēc tam ir gandrīz gatavs vietnes atklāšana. Tas, kas jums, iespējams, ir jādara, ir jāpievieno neitrālas vietnes.

Neitrālās vietnes parasti ir vietnes, kas nodrošina vienotās pierakstīšanās (SSO). Ja dodaties uz neitrālu vietni no Microsoft Edge, jūs vēlaties saglabāt pārlūkprogrammā Microsoft Edge, lai veiktu autentifikāciju. Ja pārlūkprogrammā Internet Explorer režīmā dodaties uz neitrālu vietni, jūs vēlaties, lai autentificētos Internet Explorer režīms.

Identificējiet visas SSO vai citas neitrālas vietnes, ko izmantojat, un pievienojiet tās savā uzņēmuma vietnes sarakstā.

**Internet Explorer ir noklusējuma pārlūkprogramma**

Ja tagad izmantojat tikai Internet Explorer, iespējams, nezināsit, kuras vietnes ir jauninātas uz mūsdienīgiem tīmekļa standartiem un kurām joprojām ir nepieciešama pārlūkprogramma Internet Explorer. Jūs vēlēsities atrast un pievienot šīs vietnes uzņēmuma vietņu sarakstam, lai jūs varētu izmantot Internet Explorer režīmu tikai šīm vietnēm.

> [!NOTE]
> [Uzņēmuma vietnes noteikšana](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) atklāj vietnes, kurām, iespējams, ir jāatver Internet Explorer režīms. Tas var vākt datus datoros, kuros darbojas Windows Internet Explorer 8, izmantojot Internet Explorer 11 operētājsistēmā Windows 10, Windows 8,1 vai Windows 7.

**Datu analīze**

Pēc tam, kad esat savācis vietnes datus, iesakām veikt tālāk norādītās četru soļu procesa datu analizēšanai.
1. Kārtojiet datus pēc domēna un pēc tam pēc vietrāža URL.
2. Definējiet programmas robežas, lai konfigurētu Internet Explorer režīmu. Vēlaties iekļaut visas vietnes un tīmekļa vadīklas, kas definē programmu, taču nevēlaties iekļaut papildu vietnes un vadīklas. Dažas vietnes var būt tik vienkāršas, cik *https://contoso.com/app1* savukārt citiem lietotājiem var būt nepieciešams definēt vairākas vietnes un lapas.
3. Testējiet lietojumprogrammu, lai pārliecinātos, vai tā nav nevainojama. Daudzās vietnēs tiks piedāvāts mūsdienīgs saturs, kad tie atklāj mūsdienīgu pārlūkprogrammu un piedāvā mantotu saturu tikai tad, kad tie atklāj Internet Explorer.
4. Pievienojiet programmu sarakstam uzņēmuma vietne, ja tā neveic testēšanu.

> [!NOTE]
> Kā paraugpraksi grupējiet visas vietnes, kurās ietilpst programma. Šādā veidā, jauninot programmu, ir vieglāk noņemt visu vietni no Internet Explorer režīma un sākt izmantot šīs lietojumprogrammas mūsdienīgu pārlūkprogrammu.

Kad esat pabeidzis vietnes atklāšanu un esat analizējis datus, esat gatavs sākt meklēt savā kanālu stratēģijā.

