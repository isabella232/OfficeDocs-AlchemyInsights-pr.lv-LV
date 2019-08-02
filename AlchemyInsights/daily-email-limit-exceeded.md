---
title: Ikdienas e-pasta limits pārsniegts. Darba plūsma tiks pārtraukta.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 802aba696da61be5f0a6c12072842cbc3cd96499
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059645"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Ikdienas e-pastu pārsniegts. Darba plūsma tiks pārtraukta.

Šī kļūda var saņemt šādos gadījumos:

- Darbplūsma ir SharePoint Online, kas izmanto SharePoint 2010 vai SharePoint 2013 darbplūsmas platformas tipa.
- Darbplūsma ir konfigurēta, lai nosūtītu pielāgotus e-pasta ziņu vairāk nekā 200 lietotājiem laikā, vairāk nekā 10000 adresāti dienā vai vairāk nekā 30 ziņojumi minūtē.
- Palaižot darbplūsmu, e-pasta ziņa nav nosūtīta un ievērojiet tālāk minētās darbības:
    - Darbplūsmu, izmantojot SharePoint 2013 platformas tipa, jūs pārlūkot lapu **Darbplūsmas statuss** . Darbplūsmas statusa lapā **Iekšējais statuss** ir iestatīts uz **uzsākšana**un informācijas balons parāda **nevar nosūtīt adresātam**.

Lai apietu šo problēmu, konfigurējiet darbplūsmas nosūtīt e-pasta ziņojumus bez [Exchange Online sūtītāja robežas](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)pārsniegšana. Piemēram, lietot darbplūsmas pauzi, nosūtīt e-pastu uz Office 365 grupu, adresātu grupu vai pasta iespējots drošības grupa vai nosūtītu ziņu uz mazāk nekā 200 adresātiem vienā reizē.


Lai iegūtu papildinformāciju, skatiet šādu [rakstu](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Saistītās tēmas
- [Radīt plūsmu](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint un plūsmas](https://flow.microsoft.com/blog/sharepoint-and-flow/) 