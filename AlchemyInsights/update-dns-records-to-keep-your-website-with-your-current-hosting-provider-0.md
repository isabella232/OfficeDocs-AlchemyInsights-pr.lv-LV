---
title: Saglabāt jūsu mājas lapā ar savu pašreizējo hostinga sniedzēja DNS ieraksti tiks atjaunināti
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: f2cdb319e56b82c09b7a9856c81a45e69dee6759
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/22/2019
ms.locfileid: "30760993"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Saglabāt jūsu mājas lapā ar savu pašreizējo hostinga sniedzēja DNS ieraksti tiks atjaunināti

1. Lapā [Domēni](https://portal.office.com/adminportal/home#/Domains) domēnu, sarakstā atlasiet domēna jūs izmantojat jūsu mājas lapā un pēc tam atlasiet **DNS iestatījumus** rūts vadība. 
    
2. Atlasiet **+ jaunu pielāgotu ierakstu** un ievadiet šādu formulu: 
    
  - Ievadiet **DNS tips** : **(adrese)**
    
  - **Resursdatora nosaukumu vai aizstājvārdu**, ievadiet:**@**
    
  - **IP adresi**, ierakstiet statiska IP adrese jūsu mājas lapā, kur tas pašlaik ir izvietots (piemēram, 172.16.140.1). 
    
    Šim ir jābūt *statiskā* IP adrese tīmekļa vietni, nevis *dinamisko* IP adresi. Sazinieties ar vietu, kur jūsu mājas lapā tiek izvietots, lai pārliecinātos, jūs varat saņemt statisko IP adresi jūsu publiskajā vietnē. 
    
3. Izvēlieties **Saglabāt**. 
    
Turklāt varat izveidot CNAME ierakstu, lai palīdzētu klientiem atrast jūsu mājas lapā.
  
1. Atlasiet **+ jaunu pielāgotu ierakstu** un ievadiet šādu formulu: 
    
  - Ievadiet **DNS tips** : **CNAME (aizstājvārds)**
    
  - **Resursdatora nosaukumu vai aizstājvārdu**, rakstiet sekojošo: **www**
    
  - **Norāda uz adresi**, ievadiet pilnībā kvalificētu domēna nosaukumu (FQDN) jūsu mājas lapā (piemēram, contoso.com). 
    
2. Izvēlieties **Saglabāt**. 
    

