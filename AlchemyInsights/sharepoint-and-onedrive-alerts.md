---
title: SharePoint un OneDrive brīdinājumu saņemšanas aizkave
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 27cc744bc57f1c18649e05c5b0df3b315c9c0201
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727250"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a>SharePoint un OneDrive brīdinājumu saņemšanas aizkave

- Vispirms pārbaudiet mapi Nevēlamais e-pasts.
- Ja **visi brīdinājumi no vairākiem failiem vai bibliotēkām ir aizkavēti**, apmeklējiet [Pakalpojuma darbspējas informācijas paneli](https://portal.office.com/adminportal/home?ref=/servicehealth) , lai noskaidrotu, vai nav konsultantu/starpgadījumu, kas var notikt ar SharePoint vai Exchange. Šī problēma var būt saistīta ar SharePoint brīdinājumu iespējām vai kavējumiem e-pasta ziņojumos, izmantojot Exchange. Ņemiet arī vērā, vai tiek piegādāts cits e-pasta ziņojums — ja tā nav, problēma ir iespējama ar Exchange kavējumiem.
- Ja **atsevišķa faila vai bibliotēkas brīdinājums nav piegādāts**, mēģiniet to izdzēst un izveidot no jauna. Lai atkārtoti izveidotu brīdinājumu, skatiet rakstu [SharePoint brīdinājumu pārvaldība, skatīšana un dzēšana](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) .

> [!NOTE]
> - Brīdinājumus nevar nosūtīt uz adresātu grupu. Tiek atbalstītas tikai drošības un O365 grupas.
> - Jūs nevarat pielāgot brīdinājuma e-pasta veidnes. Lai sasniegtu šos pakalpojumus, ir jāizmanto Microsoft Flow vai SharePoint Designer darbplūsma.
