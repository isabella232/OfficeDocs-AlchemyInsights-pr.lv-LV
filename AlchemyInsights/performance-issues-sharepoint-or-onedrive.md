---
title: Veiktspējas problēmas-SharePoint vai OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068416"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint vai OneDrive lēns, nepieejams vai nav pieejams vairākiem lietotājiem

SharePoint vai OneDrive var būt lēns, nepieejams vai nav pieejams, vai var parādīt pakalpojumu nav pieejams vai 503 kļūdas, vairāku iemeslu dēļ:
  
- Ja SharePoint vai OneDrive vietne ir lēna vai aizkavēta vairākiem lietotājiem, var būt pagaidu pakalpojumu problēma, kad lietotājiem rodas intermitējošas aizkaves vai navigācijas kļūdas, piekļūstot SharePoint vietnes vai OneDrive saturu. Pārbaudiet [pakalpojuma darbspējas informācijas paneli](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , lai noskaidrotu, vai jūsu organizācija ir ietekmēta.
  
- Lietotāji var saņemt *503 serveris ir aizņemts* kļūda, mēģinot naviģēt uz SharePoint vai OneDrive vietnes. Šo kļūdu var izraisīt ierobežošana SharePoint pakalpojumu ietvaros. SharePoint Online izmanto ierobežošana, lai uzturētu optimālu veiktspēju un uzticamību SharePoint Online pakalpojumu. Ierobežošana ierobežo lietotāja darbību skaitu vai vienlaicīgus zvanus (pēc skripta vai koda), lai novērstu resursu pārmērīgu izmantošanu. Lai iegūtu papildinformāciju par ierobežošana redzēt, [Izvairieties kļūst ierobežotas vai bloķēts SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Ja sistēma darbojas ļoti lēni ar **klasisko** vai **moderno** SharePoint vietni vai lapu, izmantojiet [lapu diagnostikas rīku](https://aka.ms/perftool) , lai analizētu lapas.
  
- Ja joprojām rodas vispārīga lēna veiktspēja, lūdzu, pārskatiet resursus šī raksta apakšā: [Ievads SharePoint Online veiktspējas precizēšana](https://go.microsoft.com/fwlink/?linkid=2024334)
  