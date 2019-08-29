---
title: Atjauniniet DNS ierakstus, lai uzturētu jūsu vietni ar pašreizējo viesošanas pakalpojumu sniedzēju
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 7bd36c3954d12d3ee4ac624a2f827d8e5cd88082
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665767"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Atjauniniet DNS ierakstus, lai uzturētu jūsu vietni ar pašreizējo viesošanas pakalpojumu sniedzēju

1. Microsoft 365 administrēšanas centrā pārejiet uz lapu **iestatījumu** > [Domēni](https://portal.office.com/adminportal/home#/Domains) un domēnu sarakstā atlasiet domēnu, kuru izmantojat savai vietnei.

2. Atlasiet **+ Jauns pielāgots ieraksts** un ievadiet sekojošo:

  - **DNS tipa** ievadei: **a (adrese)**

  - **Resursdatora nosaukumu vai aizstājvārdu**, ierakstiet šādu:**@**

  - Lai iegūtu **IP adresi**, ierakstiet savas vietnes statisko IP adresi, kur tā pašlaik tiek viesota (piemēram, 172.16.140.1).

    Šī ir *statiska* IP adrese mājas lapā, nevis *dinamisko* IP adresi. Pārbaudiet ar vietni, kur jūsu mājas lapā ir izvietots, lai pārliecinātos, ka jūs varat saņemt statisku IP adresi jūsu publiskajā vietnē.

3. Atlasiet **saglabāt**.

Turklāt varat izveidot CNAME ierakstu, lai palīdzētu klientiem atrast jūsu vietni.
  
1. Atlasiet **+ Jauns pielāgots ieraksts** un ievadiet sekojošo:

  - **DNS tipa** ievadiet: **CNAME (aizstājvārds)**

  - **Resursdatora nosaukumu vai aizstājvārdu**, ierakstiet šādu: **www**

  - Par **punktiem, uz adresi**, ierakstiet pilnu domēna nosaukumu (FQDN) jūsu mājas lapā (piemēram, contoso.com).

2. Atlasiet **saglabāt**.
