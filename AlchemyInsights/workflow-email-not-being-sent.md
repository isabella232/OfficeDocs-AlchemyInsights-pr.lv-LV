---
title: Darbplūsmas e-pasts netiek sūtīts
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
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748996"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Darbplūsmas e-pasts netiek sūtīts SharePoint sarakstam vai bibliotēkai

1. E-pasta ziņojumi no darbplūsmām netiek nosūtīti visiem lietotājiem vai tikai konkrētiem lietotājiem, vai arī redzat kļūdas ziņojumu, **ka e-pasta ziņojums nav nosūtīts. Pārliecinieties, vai e-pasta ziņojumam ir derīgs adresāts**.

    Pārbaudiet, vai lietotājs ir šīs vietņu kolekcijas grupā **visas personas** atļaujas (lietotāju informācijas saraksts).  Izlases tiešā vietrāža URL: https:// <tenant> . SharePoint.com/sites/ <sitename> /_layouts/15/People.aspx? MembershipGroupId = 0

    - Ja lietotājs nepastāv, pārliecinieties, vai lietotājs ir pierakstījies lapā. 
    - Ja tas ir ārējs lietotājs, pārliecinieties, vai viņa uzaicinājums ir apstiprināts.
    - Ja lietotājs pastāv atļauju grupā, pārliecinieties, vai e-pasta adrese ir pareiza.
    - Ja lietotāju e-pasta adrese šeit nav iestatīta, pēc tam izveidojiet brīdinājuma paraugu šim lietotājam, kas veic šī lietotāja konta sinhronizāciju no SharePoint lietotāju profiliem šajā vietņu kolekcijā.
 
2. E-pasta ziņojumi no darbplūsmām tiek nosūtīti vietņu kolekcijas administratoriem, bet ne citiem lietotājiem, un tiek rādīts kļūdas ziņojums, **kas aizliegts <span>https:</span>//URL/_vti_bin/Client.xvc.SP.Utilities.Utility.SendEmail**.
 

    Skatiet rakstu [piekļuve liegta, ja nosūtāt e-pasta ziņojumu SharePoint grupai](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Pārliecinieties arī, vai ir aktivizēts neaktīvs **lietotāju atļauju bloķēšanas režīms** .


## <a name="related-topics"></a>Saistītās tēmas
Vai vēlaties izmēģināt Microsoft plūsmu pakalpojumā SharePoint Online?
- [Izveidot plūsmu](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint un plūsma](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


