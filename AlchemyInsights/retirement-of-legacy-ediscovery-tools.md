---
title: Iepriekšējās paaudzes eDiscovery rīku norakstīšanas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: c4632b52dde579b7d5b2e6e15f1583300a0bd136
ms.sourcegitcommit: a7c17217c170ead24571421baaf5a14f1525b1a6
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/20/2020
ms.locfileid: "42157644"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Iepriekšējās paaudzes eDiscovery rīku norakstīšanas

Jaunā un uzlabotā e-datu atklāšanas funkcionalitātes rezultātā Microsoft 365 atbilstības centrā šādas mantotās eDiscovery rīki un commandlets tiks pensijā nākamajos mēnešos:

- [In-place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) un [oriģinālu tur](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) Exchange administrēšanas centrs.

- Exchange Online PowerShell cmdlet, kas atbalsta in-place eDiscovery un oriģinālu tur. (Šie cmdlets kopīgi identificē kā * MailboxSearch cmdlet.) Tas ietver šādu cmdlet:

    - [Jauns MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Sākuma MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Kopa MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- [Meklēšanas pastkasti](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet Exchange Online PowerShell.
- Exchange tīmekļa pakalpojumos API šādas darbības:
    - [Getsearchablepastkastēm](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [Setholdonpastkastēm](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [Getholdonpastkastēm](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Office 365 Advanced eDiscovery v 1.0](https://docs.microsoft.com/en-us/microsoft-365/compliance/office-365-advanced-ediscovery)

**Pensionēšanās grafiks**:
- April 1, 2020: jūs nevarēsiet izveidot jaunu meklēšanu un tilpnēs, bet jūs joprojām varat palaist, rediģēt un dzēst esošo meklēšanu uz savu risku. Microsoft Support vairs neatbalsta in-place eDiscovery & pieder EAC.

- Jūlijs 1, 2020: In-Place eDiscovery & tur funkcionalitāti EAC tiks ievietots tikai lasīšanas režīmā. Tas nozīmē, ka varēsit noņemt tikai esošos meklēšanas vaicājumus un aizturēšanas.

Papildinformāciju **skatiet**:

 - [Mantotā eDiscovery meklēšanas un aizturēšanas migrēt uz Microsoft 365 atbilstības centrs](https://docs.microsoft.com/en-us/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Iepriekšējās paaudzes eDiscovery rīku norakstīšanas](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [BUJ par in-place eDiscovery un oriģinālu tur](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



