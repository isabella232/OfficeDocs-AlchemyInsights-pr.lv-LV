---
title: DNS ierakstu atjaunināšana, lai savu tīmekļa vietni uzturētu ar pašreizējo viesošanas pakalpojumu sniedzēju
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: f868ce25d68f61da30d2db4de88aa83675c97857b3c1371cf2039e0b03895a64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007689"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>DNS ierakstu atjaunināšana, lai savu tīmekļa vietni uzturētu ar pašreizējo viesošanas pakalpojumu sniedzēju

1. Domēnu Microsoft 365 administrēšanas centrs dodieties uz lapu Domēnu iestatīšana un domēnu sarakstā atlasiet domēnu, ko  >  [](https://admin.microsoft.com/Adminportal#/Domains) izmantojat tīmekļa vietnei.

2. Atlasiet **+ Jauns pielāgots ieraksts** un ievadiet:

  - Sadaļā **DNS tips** ievadiet A **(adrese)**

  - Laukā **Resursdatora nosaukums vai aizstājvārds** ierakstiet šādu tekstu: **@**

  - Laukā **IP adrese** ierakstiet statisko IP adresi, kur pašlaik tiek viesota jūsu tīmekļa vietne (piemēram, 172.16.140.1).

    Tai ir jābūt  *statiskai tīmekļa*  vietnes IP adresei, nevis  *dinamiskajai*  IP adresei. Pārbaudiet vietni, kur tiek viesota jūsu tīmekļa vietne, lai pārliecinātos, vai varat iegūt statisku IP adresi jūsu publiskaajai tīmekļa vietnei.

3. Atlasiet **Saglabāt**.

Turklāt varat izveidot CNAME ierakstu, lai klientiem palīdzētu atrast jūsu tīmekļa vietni.
  
1. Atlasiet **+ Jauns pielāgots ieraksts** un ievadiet:

  - Sadaļā **DNS tips ievadiet** **CNAME (aizstājvārds)**

  - Laukā **Resursdatora nosaukums vai aizstājvārds** ierakstiet šādu informāciju: **www**

  - Laukā **Norāda uz** adresi ierakstiet savas tīmekļa vietnes pilno domēna nosaukumu (FQDN) (piemēram, contoso.com).

2. Atlasiet **Saglabāt**.
