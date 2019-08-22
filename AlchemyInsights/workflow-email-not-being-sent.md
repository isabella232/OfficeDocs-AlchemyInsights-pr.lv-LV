---
title: Darbplūsmu, e-pasts netiek nosūtīts
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
- "1586"
ms.openlocfilehash: 261fe1b1bc815dd4ad568051cfefad1e214b957e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530888"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Darbplūsmu, e-pasts netiek nosūtīts uz koplietošanas vides SharePoint sarakstā vai bibliotēkā

1. E-pastu no darbplūsmas netiek nosūtītas visiem lietotājiem vai tikai noteiktiem lietotājiem, vai jūs redzat kļūdu **, e-pasta ziņojumu nevar nosūtīt. Pārliecinieties, vai e-pasts ir derīgs adresāts**.

    Pārbaudiet, ja lietotājs atrodas vietņu kolekcijas **Visi cilvēki** atļaujas grupai (lietotāju informācijas saraksts).  Parauga tiešai URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0

    - Ja lietotājs neeksistē, pārliecinieties, vai lietotājs ir parakstīts uz lapu. 
    - Ja tas ir ārējais lietotājs, pārliecinieties, ka savu ielūgumu pieņēma.
    - Ja lietotāju grupas atļaujas, pārliecinieties, vai e-pasta adrese ir pareiza.
    - Ja šeit nav iestatīti lietotāju e-pasta adresi, pēc tam izveidojiet brīdinājuma paraugu šī lietotāja, kas liek šī lietotāja konta sinhronizācijas no lietotāju profiliem, SharePoint šai vietņu kolekcijai.
 
2. E-pastu no darbplūsmas tiek nosūtīti vietņu kolekcijas administratorus, bet ne citiem lietotājiem un redzēt kļūdas **HTTP aizliegts uz <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Sk. [Liegta piekļuve, kad sūtāt e-pasta ziņojumu SharePoint grupai](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Arī, pārliecinieties, vai **ierobežotu piekļuvi lietotāja atļauju slēgts režīmā** vietņu kolekcijas līdzekli nav aktīvs.


## <a name="related-topics"></a>Saistītās tēmas
Vēlaties izmēģināt Microsoft SharePoint Online Flow?
- [Radīt plūsmu](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint un plūsmas](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


