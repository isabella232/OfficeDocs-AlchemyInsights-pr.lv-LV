---
title: Darbplūsmas e-pasta ziņojums netiek nosūtīts
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 2caf8e0878da0049667d9a19f4488eaec4b9327fbf36be7d29dbf4b7a9c89158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072527"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Darbplūsmas e-pasta ziņojums netiek nosūtīts SharePoint sarakstam vai bibliotēkai

1. E-pasta ziņojumi no darbplūsmām netiek nosūtīti visiem vai tikai konkrētiem lietotājiem, vai arī tiek parādīts kļūdas ziņojums E-pasta ziņojumu nevar nosūtīt. Pārliecinieties, vai **e-pasta ziņojumam ir derīgs adresāts.**

    Pārbaudiet, vai lietotājs pastāv atļauju **grupā Visas personas** (lietotāju informācijas saraksts) attiecībā uz šo vietņu kolekciju.  Tiešā URL paraugs: https:// <tenant> .sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx? MembershipGroupId=0

    - Ja lietotāja nav, pārliecinieties, vai lietotājs ir pierakstījies lapā. 
    - Ja tas ir ārējais lietotājs, pārliecinieties, vai uzaicinājums ir pieņemts.
    - Ja lietotājs pastāv atļauju grupā, pārliecinieties, vai e-pasta adrese ir pareiza.
    - Ja lietotāja e-pasta adrese šeit nav iestatīta, izveidojiet šim lietotājam brīdinājuma paraugu, kas liek sinhronizēt šo lietotāja kontu no šī lietotāja SharePoint šajā vietņu kolekcijā.
 
2. E-pasta ziņojumi no darbplūsmām tiek nosūtīti vietņu kolekcijas administratoriem, bet ne citiem lietotājiem, un tiek parādīts kļūdas ziņojums **HTTP Aizliegts <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Skatiet [rakstu Piekļuve liegta, nosūtot e-pasta ziņojumu SharePoint grupai.](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)

    Pārliecinieties arī par to, **vai ierobežotās piekļuves lietotāju atļauju bloķēšanas režīma vietņu** kolekcijas līdzeklis nav aktīvs.


## <a name="related-topics"></a>Saistītās tēmas
Vai vēlaties izmēģināt Microsoft Flow programmā SharePoint Online?
- [Jaunas Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint un Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


