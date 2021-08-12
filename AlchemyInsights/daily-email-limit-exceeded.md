---
title: Pārsniegts dienas e-pasta ierobežojums. Darbplūsma ir aizturēta.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 60ddbe68298e998a4e0b271a15209efc135c80638702c98dbcb3e0b2f1554860
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914658"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Pārsniegts dienas e-pasta ierobežojums. Darbplūsma ir aizturēta.

Šī kļūda var tikt saņemta šādos scenārijos:

- Jūs izmantojat darbplūsmu programmā SharePoint Online, kas izmanto SharePoint 2010 vai SharePoint 2013 darbplūsmas platformas tipu.
- Darbplūsma ir konfigurēta, lai vienlaikus nosūtītu pielāgotu e-pasta ziņojumu vairāk nekā 200 lietotājiem, vairāk nekā 10 000 adresātu dienā vai vairāk nekā 30 ziņojumus minūtē.
- Palaižot darbplūsmu, e-pasta ziņojums netiek nosūtīts un esat pamanījis šādu darbību:
    - Darbplūsmai, izmantojot platformas SharePoint 2013, pārlūkojiet līdz **lapai Darbplūsmas** statuss. Lapā Darbplūsmas statuss iekšējā statuss **ir iestatīts** uz Sākts **,** un informācijas balons tiek **rādīts Nevar nosūtīt adresātam.**

Lai novērstu šo problēmu, konfigurējiet darbplūsmu tā, lai tā nosūtītu e-pasta ziņojumus, [nepārsniegtu Exchange Online ierobežojumus.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits) Piemēram, izmantojiet pauzi darbplūsmā, nosūtiet e-pasta ziņojumu Microsoft 365 grupai, adresātu grupai vai drošības grupai, kurā iespējots pasts, vai vienlaikus nosūtiet ziņojumu mazāk nekā 200 adresātiem.


Papildinformāciju skatiet šajā [rakstā.](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)

## <a name="related-topics"></a>Saistītās tēmas
- [Jaunas Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint un Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 