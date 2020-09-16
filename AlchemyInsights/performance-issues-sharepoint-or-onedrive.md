---
title: Veiktspējas problēmas — SharePoint vai OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771908"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint vai OneDrive lēnā, nepieejama vai nav pieejama vairākiem lietotājiem

SharePoint vai OneDrive var būt lēna, nepieejama vai nepieejama, vai var tikt parādīta pakalpojuma nepieejamība vai 503 kļūdas vairāku iemeslu dēļ:
  
- Ja jūsu SharePoint vai OneDrive vietne ir lēna vai aizkavēta vairākiem lietotājiem, iespējama īslaicīga pakalpojumu problēma, kur lietotājiem rodas neregulāras aizkaves vai navigācijas kļūdas, piekļūstot SharePoint vietnēm vai OneDrive saturam. Pārbaudiet [Pakalpojuma darbspējas informācijas paneli](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , lai noskaidrotu, vai jūsu organizācija ir ietekmēta.
  
- Mēģinot veikt navigāciju uz SharePoint vai OneDrive vietnēm, lietotāji var saņemt *503 serveri ir aizņemts* . Šo kļūdu var izraisīt ierobežošana SharePoint pakalpojumā. SharePoint Online izmanto ierobežošanu, lai uzturētu optimālu SharePoint Online pakalpojuma veiktspēju un uzticamību. Ierobežošana ierobežo lietotāju darbību vai vienlaicīgu zvanu skaitu (ar skriptu vai kodu), lai nepieļautu pārmērīgu resursu pielietojumu. Papildinformāciju par ierobežošanu skatiet rakstā Neļaujiet ierobežot [vai bloķēt pakalpojumā SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Ja rodas lēna veiktspēja ar **klasisko** vai **mūsdienīgu** SharePoint vietni vai lapu, izmantojiet [lapu diagnostikas rīku](https://aka.ms/perftool) , lai analizētu lapas.
  
- Ja joprojām rodas lēna veiktspēja, lūdzu, pārskatiet resursus šī raksta beigās: [Ievads par SharePoint Online veiktspējas uzlabošanu](https://go.microsoft.com/fwlink/?linkid=2024334)
  