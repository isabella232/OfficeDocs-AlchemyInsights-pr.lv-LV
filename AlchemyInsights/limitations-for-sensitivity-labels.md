---
title: Sensitivitātes etiķešu ierobežojumi Office programmā SharePoint un OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12451"
- "9000181"
ms.openlocfilehash: e197c43712c0ead9508a1cfdf48b51d01d2ae957649f73703f9c33733e332bf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813159"
---
# <a name="limitations-for-sensitivity-labels-for-office-files-in-sharepoint-and-onedrive"></a>Sensitivitātes etiķešu ierobežojumi Office programmā SharePoint un OneDrive

Iespējojot sensitivitātes etiķetes Office failiem SharePoint un OneDrive, ņemiet vērā prasības un ierobežojumus, kas ietver:

- SharePoint un OneDrive nevar apstrādāt dažus failus, kas atzīmēti un šifrēti no Office datora programmām, ja failos ir PowerQuery dati, pielāgoto pievienojumprogrammu dati vai pielāgotas XML daļas.
- SharePoint un OneDrive sensitivitātes etiķetes automātiski nelieto esošiem failiem, kurus jau esat šifrējis, izmantojot Azure informācijas aizsardzības (AIP) etiķetes. Lai lietotu sensitivitātes etiķetes šifrētiem failiem: 
    - Pārliecinieties, vai AIP etiķetes ir migrētas un publicētas Microsoft 365 centrā.
    - Lejupielādējiet atzīmētos failus un pēc tam augšupielādējiet tos to sākotnējā SharePoint vai OneDrive atrašanās vietā.
- Šifrētu dokumentu drukāšana netiek atbalstīta.

Papildinformāciju par ierobežojumiem skatiet [rakstā Sensitivitātes etiķešu iespējošana Office failiem SharePoint un OneDrive.](/microsoft-365/compliance/sensitivity-labels-sharepoint-onedrive-files#limitations)
