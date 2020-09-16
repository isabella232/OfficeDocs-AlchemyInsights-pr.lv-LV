---
title: Pārsniegts dienas e-pasta ierobežojums. Darbplūsma ir apturēta.
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
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731570"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Pārsniegts dienas e-pasta ierobežojums. Darbplūsma ir apturēta.

Šo kļūdu var saņemt šādos scenārijos:

- Jums ir SharePoint Online darbplūsma, kas izmanto SharePoint 2010 vai SharePoint 2013 darbplūsmas platformas tipu.
- Darbplūsma ir konfigurēta, lai vienlaikus nosūtītu pielāgotu e-pasta ziņojumu vairāk nekā 200 lietotājiem, vairāk nekā 10 000 adresātiem dienā vai vairāk nekā 30 ziņojumiem minūtē.
- Palaižot darbplūsmu, netiek nosūtīts e-pasta ziņojums, un jūs pamanīsit šādu darbību:
    - Darbplūsmā, izmantojot SharePoint 2013 platformas tipu, pārlūkojiet līdz lapai **darbplūsmas statuss** . Lapā Darbplūsmas statuss **iekšējais statuss** ir iestatīts kā **startēts**, un informācijas balons tiek rādīts **nevar nosūtīt adresātam**.

Lai novērstu šo problēmu, konfigurējiet darbplūsmu, lai nosūtītu e-pasta ziņojumus, nepārsniedzot [Exchange Online sūtītāja ierobežojumus](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Piemēram, izmantojiet pauzi darbplūsmā, nosūtiet e-pasta ziņojumu uz Microsoft 365 grupu, adresātu grupu vai pasta drošības grupu, vai sūtiet ziņu uz vairāk nekā 200 adresātiem vienlaikus.


Lai iegūtu papildinformāciju, skatiet šo [rakstu](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Saistītās tēmas
- [Izveidot plūsmu](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint un plūsma](https://flow.microsoft.com/blog/sharepoint-and-flow/) 