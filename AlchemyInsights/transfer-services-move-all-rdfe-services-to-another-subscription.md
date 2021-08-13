---
title: Pārsūtīšanas pakalpojumi — visu RDFE pakalpojumu pārvietošana uz citu abonementu
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
ms.openlocfilehash: 89217922b8b51f2548f9fff53bf80364c0e897b1d9b34bfb7016f0b0f197cf17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940070"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Pārsūtīšanas pakalpojumi — visu RDFE pakalpojumu pārvietošana uz citu abonementu

**Resursu pārvietošana**

Azure resursus var pārvietot uz citu Azure abonementu vai resursu grupu tam pašam abonementam, izmantojot Azure portālu, Azure PowerShell, Azure CLI vai REST API, lai pārvietotu resursus.

Pirms resursu pārvietošanas skatiet:

- [Kontrolsaraksts pirms resursu pārvietošanas](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Pakalpojumi, ko var pārvietot](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Kā validēt pārvietošanas](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Pakalpojumu pārvietošanas norādījumi](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Lai pārvietotu esošos resursus uz citu resursu grupu vai abonementu, varat izmantot:

- [Azure portāls](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Apmācība: [Azure resursu pārvietošana uz citu resursu grupu vai abonementu](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Azure Resursu pārvaldnieka kļūdu novēršana**

Skatiet tālāk esošos rakstus, lai uzzinātu par dažām bieži sastopamām Azure izvietošanas kļūdām un saņemtu informāciju par to atrisi. Ja nevarat atrast izvietošanas kļūdas kodu, skatiet sadaļu [Kļūdas koda atrašana.](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code)

- [Izvietošanas kļūdu novēršana](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Problēmu novēršana, pārvietojot Azure resursus uz jaunu resursu grupu vai abonementu](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Ņemiet vērā — ja vēlaties jaunināt savu Azure abonementu, piemēram, pāriet no bezmaksas uz bezmaksas abonementu, ir jākonvertē abonements.

- Lai jauninātu bezmaksas izmēģinājumversiju, skatiet rakstu Bezmaksas izmēģinājumversijas jaunināšana vai Microsoft Imagine Azure abonements [uz pay-as-you-go .](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)
- Lai mainītu apmaksātu abonementu, skatiet rakstu [Azure Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)abonementa maiņa uz citu piedāvājumu.

**Lai pievienotu vai saistītu Azure abonementu ar jūsu Azure Active Directory nomnieku:**

1. Pierakstieties un Azure portāla lapā Abonementi atlasiet [abonementu, kuru vēlaties izmantot.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)
2. Atlasiet **Mainīt direktoriju**.
3. Pārskatiet parādītos brīdinājumus un pēc tam atlasiet **Mainīt**.
4. Abonementam tiek mainīts direktorijs, un tiks parādīts ziņojums par sekmīgu darbību.
5. Izmantojiet direktorija *pārslēdzēju,* lai pārietu uz jauno direktoriju. Lai viss tiktu rādīts pareizi, var paiet līdz pat 10 minūtēm.

**Ieteiktie dokumenti**

- [Azure abonementa īpašumtiesību nodošana](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Resursu pārvietošana uz jaunu resursu grupu vai abonementu](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Resursu pārvaldība, izmantojot Azure portālu](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
