---
title: Veco e-datu atklāšanas rīku vecums
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 2315c4c651a83f0ecc78c0171f32aba13bc93f8c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727790"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Veco e-datu atklāšanas rīku vecums

Jaunajā un uzlabotajā e-datu atklāšanas funkcionalitātē Microsoft 365 atbilstības centrā tālāk norādītie mantotie e-datu atklāšanas rīki un commandlets būs novecojuši.

- Oriģinālu [e-datu atklāšanu](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) un [oriģinālu turēšanu](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) Exchange administrēšanas centrā.

- Exchange Online PowerShell cmdlet, kas atbalsta oriģinālu e-datu atklāšanu un oriģinālu turēšanu. (Šīs cmdlet tiek kopīgi identificētas kā *-MailboxSearch cmdlet.) Tas ietver šādas cmdlet:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Sākums — MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Pārtraukt-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- [Meklēšanas-pastkastes](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet pakalpojumā Exchange Online PowerShell.
- Tālāk norādītās darbības Exchange tīmekļa pakalpojumu API.
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Uzlabots e-datu atklāšanas v 1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Pensijas laika grafiks**:
- **2020. gada 1. jūlijs** Jūs vairs nevarat izveidot jaunus meklēšanas un aizturēšanas, bet jūs pats varat veikt, rediģēt un dzēst esošos meklēšanas rezultātus. Microsoft atbalsts vairs neatbalsta e-datu atklāšanu, & ir iekļauta EAC.
    
- **2020. gada 1. oktobris** Atrašanās vietas e-datu atklāšanas &ā EAC funkcionalitāte tiek iekļauta tikai lasīšanas režīmā, tāpēc varat noņemt tikai esošos meklēšanas rezultātus un aizturēšanas.

Papildinformāciju **skatiet rakstā**:

 - [Mantoto e-datu atklāšanas meklēšana un aizturēšana uz Microsoft 365 atbilstības centru](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Veco e-datu atklāšanas rīku vecums](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Bieži uzdotie jautājumi par oriģinālu e-datu atklāšanu un oriģinālu turēšanu](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



