---
title: Mantoto e-datu atklāšanas rīku norakstīšana
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798556"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Mantoto e-datu atklāšanas rīku norakstīšana

Ņemot vērā jauno un uzlaboto e-datu atklāšanas funkcionalitāti Microsoft 365 atbilstības centrā, nākamo mēnešu laikā tiks izņemti šādi mantoti e-datu atklāšanas rīki un komandlietotņi:

- [Ievietojiet e-datu atklāšanu](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) [un izteiksmju](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) glabāšanu Exchange administrēšanas centrā.

- Exchange Online PowerShell cmdlet, kas atbalsta In-Place e-datu atklāšanu un glabāšanuIn-Place aizturēšanas. (Šīs cmdlet kopā tiek identificētas kā *-MailboxSearch cmdlet.) Tas ietver šādas cmdlet:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Meklēšanas [pastkastes](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet meklētājprogrammā Exchange Online PowerShell.
- Tālāk norādītās darbības Exchange tīmekļa pakalpojumu API:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Pensijas laika grafiks:**
- **2020. gada 1. jūlijs** Jūs vairs nevarat izveidot jaunus meklējumus un aizturēšanu, tomēr jūs varat veikt, rediģēt un dzēst esošos meklēšanas vaicājumus uz savu risku. Microsoft atbalsta dienests vairs neatbalsta In-Place e-& glabāšanu EAC.
    
- In-Place. gada **1.** oktobris & e-datu atklāšanas līdz ar & aizturēšanas funkcionalitāti EAC tiks novietota tikai lasīšanas režīmā, tāpēc varat noņemt tikai esošās meklēšanas un aizturēšanas.

**Papildinformāciju skatiet rakstā:**

 - [Mantoto e-datu atklāšanas meklējumu migrēšana uz Microsoft 365 atbilstības centru](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Mantoto e-datu atklāšanas rīku norakstīšana](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Bieži uzdotie jautājumi In-Place e-datu atklāšanu In-Place aizturēšanu](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



