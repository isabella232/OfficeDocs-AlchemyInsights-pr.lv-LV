---
title: Pakalpojumu pārsūtīšana — visu RDFE pakalpojumu pārvietošana uz citu abonementu
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692169"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Pakalpojumu pārsūtīšana — visu RDFE pakalpojumu pārvietošana uz citu abonementu

**Pārvietot resursus**

Azure resursus var pārvietot uz citu Azure abonementu vai resursu grupu zem tā paša abonementa, izmantojot Azure Portal, Azure PowerShell, Azure CLI vai REST API, lai pārvietotu resursus.

Lai varētu pārvietot resursus, skatiet:

- [Kontrolsaraksts pirms resursu pārvietošanas](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Pakalpojumi, kurus var pārvietot](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Kā validēt pārvietošanu](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Norādījumi par pakalpojumu pārvietošanu](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Lai pārvietotu esošos resursus uz citu resursu grupu vai abonementu, varat izmantot:

- [Azure Portal](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Apmācība: [Azure resursu pārvietošana uz citu resursu grupu vai abonementu](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Problēmu novēršana saistībā ar Azure Resource Manager**

Skatiet tālāk norādītos rakstus, lai uzzinātu par dažām tipiskām Azure izvietošanas kļūdām un saņemtu informāciju par to atrisināšanu. Ja nevarat atrast kļūdas kodu jūsu izvietošanas kļūdai, skatiet tēmu [kļūdas koda atrašana](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [Izvietošanas kļūdu novēršana](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Problēmu novēršana, pārvietojot Azure resursus uz jauno resursu grupu vai abonementu](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Ņemiet vērā, ka, ja vēlaties jaunināt savu Azure abonementu, piemēram, pārejat no bezmaksas uz Pay-you-go, ir jākonvertē savs abonements.

- Lai jauninātu bezmaksas izmēģinājumversiju, skatiet rakstu [bezmaksas izmēģinājumversijas vai Microsoft Imagine Azure abonementa jaunināšana uz Pay-you-go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).
- Lai mainītu apmaksas-as-Go kontu, skatiet rakstu [Azure pay-as-Go abonementa maiņa uz citu piedāvājumu](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).

**Lai pievienotu vai asociētu Azure abonementu Azure Active Directory nomniekam:**

1. Pierakstieties un atlasiet abonementu, kuru vēlaties izmantot [Azure portāla lapā abonementi](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).
2. Atlasiet **mainīt direktoriju**.
3. Pārskatiet brīdinājumus, kas tiek parādīti, un pēc tam atlasiet **mainīt**.
4. Direktorijs ir mainīts abonementam, un jūs saņemsit ziņojumu par veiksmīgu izdošanos.
5. Izmantojiet *direktoriju* pārslēdzēju, lai pārietu uz jauno direktoriju. Lai viss tiktu rādīts pareizi, var būt nepieciešamas līdz pat 10 minūtēm.

**Ieteicamie dokumenti**

- [Azure abonementa īpašumtiesību nodošana](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Pārvietot resursus uz jauno resursu grupu vai abonementu](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Resursu pārvaldība, izmantojot Azure Portal](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
