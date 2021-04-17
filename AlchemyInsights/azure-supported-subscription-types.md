---
title: Atbalstītie abonementu tipi
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
- "6675"
ms.openlocfilehash: dcf5855bff8725ea746196c1f07d689ce1797f8c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820689"
---
# <a name="supported-subscription-types"></a>Atbalstītie abonementu tipi

Lūdzu, pirms turpināt, pārskatiet atbalstītos abonementu tipus.

[Atbalstītie abonementu tipi](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Norēķinu tiesību nodošana**

Pierakstieties Azure portālā kā [administrators norēķinu kontā](https://ms.portal.azure.com/), kuram ir abonements, kuru vēlaties nodot.

- Meklējiet atslēgas vārdus **Izmaksu pārvaldība + Norēķini**. Kreisajā rūtī atlasiet **Abonementi**. Atkarībā no piekļuves veida, jums varētu būt nepieciešamas atlasīt norēķinu tvērumu un pēc tam **Abonementi** vai **Azure abonementi**.
- Atlasiet Nodot norēķinu tiesības nododamajam abonementam.
- Ievadiet lietotāja, kas būs jaunais abonementa norēķinu administrators, e-pasta adresi un pēc tam atlasiet **nosūtīt nodošanas pieprasījumu**.
- Lietotājs saņems e-pastu ar norādījumiem jūsu nodošanas pieprasījuma pārskatīšanai. Lai apstiprinātu nodošanas pieprasījumu, lietotājam ir jāatlasa e-pasta iekļautā saite un jāseko norādījumiem.

Piezīme:nododot jūsu abonementu lietotāja kontam pie cita Azure AD nomnieka, visas [lomu piekļuves vadības (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) piešķires resursu pārvaldībai abonementā tiks neatgriezeniski noņemtas. Tikai jaunajam īpašniekam būs piekļuve abonementa resursu pārvaldībai. Papildinformācijai lasiet [Abonementa nodošana cita Azure AD nomnieka lietotājam](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Abonementa īpašumtiesību nodošana**

Abonementa īpašumtiesību nodošanai ir nepieciešama lomu piekļuves vadības (RBAC) loma, lai pārvaldītu resursus, ja abonements zaudēs piekļuvi. Papildinformācijai par esošā abonementa pievienošanu nomniekam lasiet [Azure abonementa piesaiste vai pievienošana Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- Abonementu ar neapmaksātu summu pašreizējā apmaksas ciklā īpašumtiesības netiks pievienotas jaunā konta maksājuma instrumentam. Vienīgā informācija, kas būs pieejama jaunā konta lietotājiem, ir tikai jūsu abonementa iepriekšējā mēneša cena.  Pārējie lietojuma un norēķinu vēstures dati netiek nodoti kopā ar abonementu.
- Enterprise līguma (EA) abonementu norēķinu īpašumtiesību nodošana pašlaik tiek atbalstīta tikai Enterprise līguma portālā
- Uz kredītu pamata veidotos abonementu, piemēram, Visual Studio, BizSpark, Microsoft partneru tīkls nodošanai jauniem lietotājiem ir nepieciešama Visual Studio/Microsoft partneru tīkla licence, lai pieņemtu nodošanas pieprasījumu
- Visi resursi, piemēram, virtuālās mašīnas, diski un vietnes tiks veiksmīgi nodotas jaunajam kontam. Tālāk minētos resursus var ietekmēt abonementa nodošana starp nomniekiem:

**Azure AD domēna pakalpojumi**

Azure atslēgu glabātuves

- Var tikt ietekmētas [ar SQL saistītie lietotāji un datu bāzes](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support), it īpaši, ja klients izmanto ar Azure Active Directory saistīto autentifikāciju.
- Var tikt ietekmēti **lietojumprogrammu pakalpojumi**, kas ir konfigurēti ar Azure Active Directory autentifikāciju
- **Visual Studio Team** pakalpojumu konti, kas ir saistīti ar Azure abonementiem, var īslaicīgi zaudēt piekļuvi brīdī, kad tiek atcelts Azure abonements

**Ieteiktie dokumenti**

Darbības pēc norēķinu īpašumtiesību pieņemšanas:

- Lai saglabātu norēķinu īpašumtiesības, bet mainītu jūsu abonementa tipu, lasiet: [Piedāvājums mainīt Azure abonementu](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Visual Studio, Microsoft Partner Network (MPN) un Pay as you go Dev/Test abonementi](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Enterprise līguma (EA) norēķinu īpašumtiesību nodošana](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [BUJ par īpašumtiesību nodošanu](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Īpašumtiesību nodošanas problēmu novēršana](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)