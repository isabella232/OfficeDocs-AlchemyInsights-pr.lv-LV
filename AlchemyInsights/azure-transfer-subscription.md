---
title: Nodot Azure norēķinu tiesības
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6849"
ms.openlocfilehash: fc02a64807cad61cfeecf04d1f8e38666402583f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820617"
---
# <a name="transfer-azure-billing-ownership"></a>Nodot Azure norēķinu tiesības

Pierakstieties [Azure portālā](https://portal.azure.com/) kā administrators norēķinu kontā, kuram ir abonements, kuru vēlaties nodot. Ja neesat pārliecināti, vai esiet administrators, vai jums ir jānosaka, kas ir administrators, lasiet [Norēķinu konta administratora noteikšana](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

1. Meklējiet atslēgas vārdus _Izmaksu pārvaldība + Norēķini_.
1. Kreisajā rūtī atlasiet **Abonementi**. Atkarībā no piekļuves veida, jums varētu būt nepieciešamas atlasīt norēķinu tvērumu un pēc tam **Abonementi** vai **Azure abonementi**.
1. Atlasiet **Nodot norēķinu tiesības** nododamajam abonementam.
1. Ievadiet lietotāja, kas būs jaunais abonementa norēķinu administrators, e-pasta adresi un pēc tam atlasiet **nosūtīt nodošanas pieprasījumu**.
1. Lietotājs saņems e-pastu ar norādījumiem jūsu nodošanas pieprasījuma pārskatīšanai. Lai apstiprinātu nodošanas pieprasījumu, lietotājam ir jāatlasa e-pasta iekļautā saite un jāseko norādījumiem.

Lūdzu, ņemiet vērā, ka, nododot jūsu abonementu lietotāja kontam pie cita Azure AD nomnieka, visas [lomu piekļuves vadības (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) piešķires resursu pārvaldībai abonementā tiks neatgriezeniski noņemtas. Tikai jaunajam īpašniekam būs piekļuve abonementa resursu pārvaldībai. Papildinformācijai par abonementa direktorija maiņu, lasiet [Abonementa nodošana cita Azure AD nomnieka lietotājam](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

_**Būtiska ietekme uz jūsu rēķiniem**_: ja nodevāt Azure abonementa norēķinu tiesības, piemērotā maksa tiks dalīta proporcionāli. Jūs varēsit piekļūt rēķiniem šādi:  

1. Atlasiet abonementu  [Abonementu lapā](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) Azure portālā [kā lietotājs ar piekļuvi rēķiniem](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support), pēc tam atlasiet **Rēķini**.
1. Noklikšķiniet **Lejupielādēt rēķinu**, lai apskatītu jūsu rēķina PDF kopiju. Ja tiek parādīts ziņojums _Nav pieejams_, tad lasiet [Kāpēc es neredzu rēķinu par pēdējo norēķinu periodu?](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice).
1. Jūs varat apskatīt lietojumu pa dienām, noklikšķinot uz **norēķinu periods**, lai iegūtu jūsu rēķinu PDF failā un failu (.CSV) ar detalizētu informāciju par lietojumu pa dienām. Papildinformācijai lasiet  [Iegūt rēķinu un lietojuma datus](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support).

**Ieteiktie dokumenti**

- [Azure abonementa norēķina tiesību nodošana citam kontam](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Par Azure abonementa norēķinu tiesību nodošanu](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Visual Studio, Microsoft Partner Network (MPN) un Pay as you go Dev/Test abonementi](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [BUJ par īpašumtiesību nodošanu](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Īpašumtiesību nodošanas problēmu novēršana](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
