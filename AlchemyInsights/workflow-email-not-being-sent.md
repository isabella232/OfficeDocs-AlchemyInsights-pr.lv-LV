---
title: Darbplūsmas e-pasts netiek sūtīts
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 391d3a2dcc2676a405065115f375c802d2492119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766140"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Darbplūsmas e-pasta netiek nosūtīts SharePoint saraksta vai bibliotēkas

1. E-pasta ziņojumi no darbplūsmas netiek sūtīti visiem lietotājiem vai tikai konkrētiem lietotājiem, vai arī tiek parādīts kļūdas ziņojums **nevar nosūtīt e-pasta ziņojumu. Pārliecinieties, vai e-pastam ir derīgs adresāts**.

    Pārbaudiet, vai lietotājs ir vietņu kolekcijas **visas personas** atļaujas grupas (lietotāja informācijas saraksts).  Paraugs Direct URL: https://<tenant>. sharepoint.com/sites/<sitename>/_layouts/15/People.aspx? MembershipGroupId = 0

    - Ja lietotājs neeksistē, pārliecinieties, vai lietotājs ir pierakstījies lapā. 
    - Ja tas ir ārējais lietotājs, pārliecinieties, vai viņu uzaicinājums ir akceptēts.
    - Ja lietotājs pastāv atļauju grupas, pārliecinieties, vai e-pasta adrese ir pareiza.
    - Ja lietotājiem e-pasta adrese nav iestatīta šeit, pēc tam izveidojiet parauga brīdinājumu šim lietotājam, kas liek sinhronizēt šo lietotāja kontu no SharePoint lietotāju profiliem šajā vietņu kolekcijā.
 
2. E-pasta ziņojumu no darbplūsmas tiek nosūtīti vietņu kolekcijas administratoriem, bet ne citiem lietotājiem un skatiet kļūdas **http aizliegts <span>https:</span>//URL/_vti_bin/Client.xvc.SP.Utilities.Utility.SendEmail**.
 

    [Ja nosūtāt e-pasta ziņojumu SharePoint grupai](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups), skatiet sadaļu piekļuve liegta.

    Arī pārliecināties, ka **ierobežotas piekļuves lietotāja atļaujas noslēgšanas režīmā** vietņu kolekcijas līdzeklis nav aktīvs.


## <a name="related-topics"></a>Saistītās tēmas
Vai vēlaties izmēģināt Microsoft Flow pakalpojumā SharePoint Online?
- [Izveidot plūsmu](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint un plūsmas](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


