---
title: Atbalstītie abonementu tipi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6675"
ms.openlocfilehash: 46bc60435c3f8477e9f274d90c39d0f1c6a523c6
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807566"
---
# <a name="supported-subscription-types"></a>Atbalstītie abonementu tipi

Lai turpinātu, lūdzu, pārskatiet atbalstīto abonementu tipus.

[Atbalstītie abonementu tipi](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Norēķinu īpašumtiesību nodošana**

Azure Portal kā norēķinu konta [administratora konts](https://ms.portal.azure.com/) , kura abonementu vēlaties pārsūtīt

- Meklējiet par **Cost Management + norēķiniem** . Atlasiet **abonementi** no kreisās rūts. Atkarībā no programmas Access, iespējams, būs jāatlasa norēķinu tvērums un pēc tam **abonementi** vai **Azure abonementi** .
- Atlasiet pārsūtīt norēķinu īpašumtiesības abonementam, kuru vēlaties pārsūtīt
- Ievadiet tā lietotāja e-pasta adresi, kurš ir tā konta norēķinu administrators, kas būs jaunais abonementa īpašnieks, un pēc tam atlasiet **Sūtīt pārsūtīšanas pieprasījumu**
- Lietotājs saņem e-pasta ziņojumu ar norādījumiem par pārsūtīšanas pieprasījuma pārskatīšanu. Lai apstiprinātu pārsūtīšanas pieprasījumu, lietotājs atlasa saiti e-pasta ziņojumā un seko instrukcijām.

Ņemiet vērā: Ja pārsūtāt norēķinu īpašumtiesības uz lietotāja kontu citā Azure AD nomniekā, visi [lomu piekļuves vadības (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) uzdevumi, lai pārvaldītu abonementa resursus, tiek neatgriezeniski noņemti. Tikai jaunajam īpašniekam būs piekļuve pārvaldīt resursus abonementā. Lai iegūtu papildinformāciju, skatiet rakstu [abonementa pārsūtīšana lietotājam citā AZURE ad nomniekā](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Abonementa īpašumtiesību nodošana**

Abonementa īpašumtiesību nodošanas priekšnosacījumi lomai, kuras pamatā ir piekļuve (RBAC), lai pārvaldītu šī abonementa resursus, zaudē piekļuvi. Lai iegūtu papildinformāciju par esošā abonementa pievienošanu nomniekam, skatiet rakstu [Azure Active Directory saistīšana vai pievienošana Azure pakalpojumam](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- Abonementa pārsūtīšana ar pašreizējā norēķinu cikla nenomaksāto summu netiks pārsūtīta uz jauno maksājumu instrumentu jaunajā kontā. Vienīgā informācija, kas ir pieejama lietotājiem jaunajā kontā, ir pēdējā mēneša maksa par jūsu abonementu. Pārējā lietojuma un norēķinu vēsture netiek pārsūtīta kopā ar abonementu.
- Norēķinu īpašumtiesību nodošana uzņēmuma līguma (EA) abonementiem pašlaik tiek atbalstīta tikai uzņēmuma līgumu portālā
- Uz kredītu orientēta abonementa, piemēram, Visual Studio, BizSpark, Microsoft partnera tīkla uz jaunu lietotāju pārsūtīšanai ir jābūt Visual Studio/Microsoft partnera tīkla licencei, lai akceptētu pārsūtīšanas pieprasījumu
- Visi resursi, piemēram, virtuālās mašīnas, diski un tīmekļa vietnes, tiek sekmīgi pārsūtīti uz jauno kontu. Vairāku nomnieku abonementa pārsūtīšanā var tikt ietekmēti šādi resursi:

**Azure AD domēna pakalpojumi**

Azure taustiņu glabātavas

- Ar [SQL saistīto lietotāju un datu bāzu](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) ietekmi var ietekmēt, it īpaši, ja klients izmanto Azure Active Directory saistīto autentifikāciju
- Ar Azure Active Directory autentifikāciju konfigurētie **lietojumprogrammu pakalpojumi** var tikt ietekmēti
- **Visual Studio komanda** Pakalpojumu konti, kas saistīti ar Azure abonementiem, var īslaicīgi zaudēt piekļuvi, kad ir atcelts pievienots Azure abonements

**Ieteicamie dokumenti**

Darbības pēc norēķinu īpašumtiesību akceptēšanas:

- Lai saglabātu norēķinu īpašumtiesības, bet mainītu abonementa veidu, skatiet: [Azure abonementa pārslēgšana uz citu piedāvājumu](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Visual Studio, Microsoft partneru tīkla (MPN) un pay as Go Dev/Test abonementu pārsūtīšana](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Norēķinu īpašumtiesību nodošana uzņēmumu līgumu (EA) abonementiem](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Bieži uzdotie jautājumi par īpašumtiesību nodošanu](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Īpašumtiesību nodošanas problēmu novēršana](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)