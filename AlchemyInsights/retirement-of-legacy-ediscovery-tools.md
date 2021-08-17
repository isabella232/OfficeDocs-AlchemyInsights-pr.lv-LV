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
ms.openlocfilehash: 2e7f898ac1a9e9469f633192be18e2a3a362023c83c9e510593196b5a4a0daf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074681"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Mantoto e-datu atklāšanas rīku norakstīšana

Ņemot vērā jauno un uzlaboto e-datu atklāšanas funkcionalitāti Microsoft 365 atbilstības centrā, nākamo mēnešu laikā tiks pārtraukti šādi mantoti e-datu atklāšanas rīki un komandlietotņi:

- [Ievietojiet e-datu atklāšanu](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) [un izteiksmju](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) glabāšanu Exchange centrā.

- PowerShell Exchange Online komandas, kas atbalsta In-Place e-datu atklāšanu un In-Place aizturēšanas. (Šīs cmdlet kopā tiek identificētas kā *-MailboxSearch cmdlet.) Tas ietver šādas cmdlet:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Cmdlet [Search-Mailbox programmā](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) Exchange Online PowerShell.
- Tālāk norādītās darbības Exchange tīmekļa pakalpojumu API:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Pensijas laika grafiks:**
- **2020. gada 1. jūlijs** Jūs vairs nevarat izveidot jaunus meklējumus un aizturēšanu, tomēr jūs varat veikt, rediģēt un dzēst esošos meklēšanas vaicājumus uz savu risku. Microsoft atbalsta dienests vairs neatbalsta In-Place e-& glabāšanu EAC.
    
- In-Place. gada **1.** oktobris & e-datu atklāšanas līdz ar & aizturēšanas funkcionalitāti EAC tiks novietota tikai lasīšanas režīmā, tāpēc varat noņemt tikai esošās meklēšanas un aizturēšanas.

**Papildinformāciju skatiet rakstā:**

 - [Mantoto e-datu atklāšanas meklēšanu un aizturēšanu migrēšana uz Microsoft 365 atbilstības centrs](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Mantoto e-datu atklāšanas rīku norakstīšana](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Bieži uzdotie jautājumi In-Place e-datu atklāšanu In-Place aizturēšanu](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



