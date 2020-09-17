---
title: DNS ierakstu atjaunināšana, lai savu tīmekļa vietni uzturētu ar pašreizējo viesošanas pakalpojumu sniedzēju
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 1d8654bc2dfb9063d0203992d624285eb646027d
ms.sourcegitcommit: 78939b01579b626b147d356045a37aec1170c948
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47815792"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>DNS ierakstu atjaunināšana, lai savu tīmekļa vietni uzturētu ar pašreizējo viesošanas pakalpojumu sniedzēju

1. Microsoft 365 administrēšanas centrā dodieties uz lapu **iestatīšanas**  >  [Domēni](https://admin.microsoft.com/Adminportal#/Domains) un domēnu sarakstā atlasiet tīmekļa vietnei izmantojamo domēnu.

2. Atlasiet **+ Jauns pielāgots ieraksts** un ievadiet šādu informāciju:

  - Sadaļā **DNS tips** ievadiet: **a (adrese)**

  - Sadaļā **resursdatora nosaukums vai aizstājvārds**ierakstiet šādu informāciju: **@**

  - Sadaļā **IP adrese**ierakstiet statisko IP adresi savai tīmekļa vietnei, kur tā pašlaik tiek viesota (piemēram, 172.16.140.1).

    Šai tīmekļa vietnei ir jābūt  *statiskai*  IP adresei, nevis  *dinamiskajai*  IP adresei. Lai pārliecinātos, vai jūsu publiskajai tīmekļa vietnei varat iegūt statisku IP adresi, skatiet vietni, kurā tiek viesota jūsu tīmekļa vietne.

3. Atlasiet **Saglabāt**.

Turklāt varat izveidot CNAME ierakstu, lai klientiem palīdzētu atrast jūsu tīmekļa vietni.
  
1. Atlasiet **+ Jauns pielāgots ieraksts** un ievadiet šādu informāciju:

  - Sadaļā **DNS tips** ievadiet **CNAME (aizstājvārds)**

  - Sadaļā **resursdatora nosaukums vai aizstājvārds**ierakstiet šādu informāciju: **www**

  - **Punktos uz adresi**ierakstiet savas tīmekļa vietnes pilno domēna nosaukumu (FQDN) (piemēram, contoso.com).

2. Atlasiet **Saglabāt**.
