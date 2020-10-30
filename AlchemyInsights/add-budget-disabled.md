---
title: Kāpēc poga Pievienot budžetu ir atspējota man?
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
- "9003547"
- "6464"
ms.openlocfilehash: 18edad73f617ba180cb08576ee6e5fa8faf07128
ms.sourcegitcommit: 9a7b85eae0bb775bc2498a83d8f5fedb72a6451e
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807412"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Kāpēc poga Pievienot budžetu ir atspējota man?

Lai izveidotu budžetu, jums ir jābūt kādai no tālāk norādītajām atļaujām.

- Pārvaldības grupa, abonements, resursu grupas tvērumi
- Izmaksu pārvaldības līdzstrādnieks
- Īpašnieks
- Līdzstrādnieks
- Tikai uzņēmuma klients: reģistrācija, nodaļa, kontu tvērumi
- Reģistrācijas administrators (iestatīt budžetu pēc reģistrācijas apjoma)
- Nodaļas administrators (iestatīt budžetu nodaļas tvērumā)
- Konta īpašnieks (iestatīt budžetu pēc konta tvēruma)
- Mūsdienīgs klienta līgums: norēķinu konts, norēķinu profils, rēķinu sadaļu tvērumi
- Azure abonēšanas veidotājs

**Es izveidoju budžetu, kad manas izmaksas par pašreizējo mēnesi jau pārsniedza budžetu. Kāpēc nesaņēmu brīdinājumu?**  
Ja jums jau ir pārsniegts noteiktais izmaksu slieksnis, kad izveidojat budžetu, ko brīdinājums neaizdegsies. Tiklīdz jaunais cikls sāksies, ja pārtrauksit slieksni, brīdinājums tiek uzkurināts.

**Kad gaidīt saņemt brīdinājumu pēc tam, kad būšu pārsniedzis kādu no maniem definētajiem budžeta brīdinājumu sliekšņiem?**  
Budžeti tiek novērtēti ik pēc 4 stundām. Lietojuma datiem ir nepieciešamas vismaz 8 stundas, lai sasniegtu budžetu sistēmu. Ņemot vērā šo, brīdinājumi var ilgt līdz 12 stundām pēc sliekšņa pārsniegšanas.

**Kāpēc, atlasot mēneša vai norēķinu mēneša atiestates periodu, ir atspējota poga sākuma datums?**  
Budžeti tiek līdzināti uz pašreizējo kalendāra mēnesi vai pašreizējo norēķinu periodu (ja ir atlasīts norēķinu mēnesis). Tāpēc šī vērtība ir iepriekš aizpildīta.

**Kāpēc budžeta izveides pieredzē nav redzama mana izmaksu grafika?**  
Lai varētu izveidot diagrammu, kas jums palīdzēs ar budžeta izveidi, mums ir nepieciešami vismaz 2 mēnešus.

**Kāpēc nevaru iestatīt budžetu uz tikko izveidoto abonementu?**  
Pēc abonementa izveides datu darbība ilgst 24-48 stundas, pirms tiek iestatīts budžets pret to.

**Budžeta API resursi**

- [Budžets API V1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): nodrošina darbības, lai izveidotu un atjauninātu budžetus. Izmantojot API budžeti, varat iestatīt budžeta slieksni un konfigurēt vairākus brīdinājumus, lai tie tiktu palaisti, kad tuvojas šis slieksnis. Brīdinājumi var izraisīt e-pasta vai Azure darbību grupu, lai veiktu automatizāciju. Piezīme. Šī API filtrēšana netiek līdzināta ar vaicājumu API filtrēšanu/dimensijām.
- [Budžeti API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): izveidojiet budžetu ar lielākām izmaksu filtrēšanas iespējām nekā V1. Filtrēšana tiek līdzināta atbilstoši mūsu vaicājumu un dimensiju API izmantotajam līgumam. Šis ir ieteicamais budžets API, kas jāizmanto, lai pārietu uz priekšu.
- [Dimensions](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): nodrošina darbības, lai iegūtu atbalstītos izmērus jūsu lietojumam dažādos tvērumos. Izmantojot dimensiju API, varat izgūt to dimensiju sarakstu, ko var izmantot kā ievades vaicājumu ģenerēšanai ar vaicājuma API.
- [Vaicājums](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): nodrošina darbības, lai iegūtu apkopotu izmaksas un lietojuma datus, pamatojoties uz jūsu sniegto vaicājumu. Izmantojot vaicājumu API, varat norādīt vēlamo filtrēšanu, kārtošanu un grupēšanu visās pieejamajās dimensijās (kam piekļūst no izmēriem API).

**Prognozētās izmaksas**

**Kāpēc es neredzu prognozes par izmaksām izmaksu analīzē?**  
Pastāv vairāki iemesli, kāpēc, veicot izmaksu analīzi, trūkst prognozes prognozes, daži no tiem ir šādi:

1. Ja jūsu izmaksas dati ir jaunāki par 10 dienām, prognozes diagramma netiks ielādēta. Modelim ir nepieciešamas vismaz 10 dienas no pēdējiem izmaksu datiem precīzas prognozes
2. Ja ir atlasīti vēsturiskie datumi, prognozes diagramma nebūs redzama. Lūdzu, atlasiet datumu diapazonu, kurā tiks parādīti prognozes diagrammas nākamie datumi
3. Ja jūsu kontam ir vairākas valūtas, prognozes diagramma sedz tikai projekta izmaksas par "visām izmaksām USD"

**Kāpēc prognozes netiek mainītas, kad veicu izmaiņas manos resursos?**  
Prognozes modelim ir nepieciešamas pāris dienas, lai kontā veiktu izmaiņas kontā, un neveic tūlītējus projekcijas, pamatojoties uz izmaiņām resursos.  
Lai palielinātu vai samazinātu resursu palielināšanas darbības, modelim ir nepieciešams mazliet ilgāks laiks, lai pielāgotos šīm izmaiņām kontā, kas nav anomālijas

**Kāpēc mana prognoze palielinās pēc rezervācijas vai Marketplace iegādes?**  
Prognozes modelī ir ņemta vērā jūsu faktiskā pašizmaksa, un tas nenodrošina izmantošanu un iegādi atsevišķi. Vienreizēja pirkuma gadījumā modelis samazinās prognozes pēc 10 dienām, lai pieskaitītu pēkšņo izmaksu pieaugumu

**Vēlos redzēt prognozes vienai dimensijai (piemēram,. Mērītājs**  
Prognoze pašlaik atbalsta kopējās izmaksu prognozes, nevis atsevišķiem skaitītājiem. Līdz ar to, kad ir sagrupēts pēc dimensijas, prognozes būs visu dimensiju vienumu kopskaits

**Ieteicamie dokumenti**

- [Kas ir Azure izmaksu pārvaldība?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure izmaksu pārvaldības labākā prakse](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Izmaksu un izdevumu analīze](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Pētīt un analizēt izmaksas ar izmaksu analīzi](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure izmaksu pārvaldība: cenas](https://azure.microsoft.com/services/cost-management/#pricing)
- [Izmaksu analīzes izmaksas](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Video apmācība: budžeta izveide Azure portālā](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Budžeta skatīšanas un pielāgošanas priekšnoteikumi](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Budžetu izveide un pārvaldība](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Automatizācijas konfigurēšana, izmantojot Azure darbību grupas un budžetu API](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Izmaksu brīdinājumu izmantošana, lai pārraudzītu lietojumu un tēriņus](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Izmaksu pārvaldības paraugprakse](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Apmācības video**

- [Budžeta izveide Azure portālā](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Pārvaldīt izmaksas ar budžetu API un darbību grupām](https://go.microsoft.com/fwlink/?linkid=2147038)