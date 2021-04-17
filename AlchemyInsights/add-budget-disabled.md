---
title: Kāpēc man ir atspējota poga Pievienot budžetu?
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
- "9003547"
- "6464"
ms.openlocfilehash: 426a54ea22490dcc47f40fd990654b2cf051a058
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822642"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Kāpēc man ir atspējota poga Pievienot budžetu?

Lai izveidotu budžetu, nepieciešama kāda no šīm atļaujām:

- Pārvaldības grupa, abonements, resursu grupas tvērumi
- Cost Management Contributor
- Īpašnieks
- Līdzstrādnieks
- Tikai Enterprise klients: Reģistrācija, Nodaļa, Konta tvērumi
- Reģistrācijas administrators (iestatīt budžetu reģistrācijas tvērumā)
- Nodaļas administrators (iestatīt budžetu nodaļas tvērumā)
- Konta īpašnieks (budžeta iestatīšana konta tvērumā)
- Tikai modernais klientu līgums: Norēķinu konts, norēķinu profils, rēķinu sadaļu tvērumi
- Azure abonementa veidotājs

**Es izveidoju budžetu, ja pašreizējā mēneša izmaksas jau bija pārsniedzis budžetu. Kāpēc es nesaņēma brīdinājumu?**  
Ja jau esat pārsniedzis norādīto izmaksu slieksni, kad izveidojat brīdinājumu par budžetu, šis brīdinājums netiks atlaists. Tiklīdz sākas jauns cikls, ja pārsniegsiet slieksni, brīdinājums tiks atlaists.

**Kad ir paredzams, ka saņemsit brīdinājumu, kad pārsniegšu kādu no maniem definētajiem budžeta brīdinājumu sliekšņiem?**  
Budžeti tiek novērtēti ik pēc 4 stundām. Lai lietojuma dati sasniegtu budžeta sistēmu, ir nepieciešamas vismaz 8 stundas. Pēc šī brīdinājuma pārsniegšanas var paiet pat 12 stundas, līdz pārsniegsiet slieksni.

**Kāpēc poga Sākuma datums ir atspējota, kad atlasu mēneša vai norēķinu mēneša atiestatīšanas periodu?**  
Budžeti ir saskaņoti ar pašreizējo kalendāra mēnesi vai pašreizējo norēķinu periodu (gadījumā, ja ir atlasīts Norēķinu mēnesis). Tāpēc mēs iepriekš aizpildajam šo vērtību jūsu lietošanai.

**Kāpēc es neredzu savu izmaksu diagrammu budžeta izveides pieredzē?**  
Lai varētu atveidot diagrammu, kas palīdzēs izveidot budžetu, mums ir nepieciešami vismaz 2 mēnešu izmaksu dati.

**Kāpēc es nevaru iestatīt budžetu tikko izveidotam abonementam?**  
Pēc abonementa izveides dati tiek apstrādāti 24–48 stundas pirms budžeta iestatīšanas.

**Budžeta API resursi**

- [Budžeta API v1 :](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support)nodrošina darbības, lai izveidotu un atjauninātu budžetus. Izmantojot budžeta API, varat iestatīt budžeta slieksni un konfigurēt vairākus brīdinājumus, lai tie parādītos, tuvojoties šim slieksnim. Brīdinājumi var aktivizēt e-pasta ziņojumu vai Azure darbību grupu, lai veiktu automatizāciju. Piezīme. Šī API filtrēšana netiek izlīdzināta ar vaicājuma API filtrēšanu/dimensijām.
- [Budgets API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): Izveidojiet budžetus ar lielākām izmaksu filtrēšanas iespējām nekā v1. Filtrēšana atbilst mūsu vaicājumu un dimensiju API izmantotajiem līgumiem. Šis ir ieteicamais budžeta API pārvietošanai uz priekšu.
- [Dimensijas](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): nodrošina darbības, lai iegūtu atbalstītās dimensijas jūsu lietojumam dažādos tvērumos. Izmantojot dimensiju API, varat izgūt dimensiju sarakstu, ko var izmantot kā ievadi vaicājumu ģenerēšanas vaicājumiem, izmantojot vaicājuma API.
- [Vaicājums:](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support)nodrošina darbības, lai iegūtu apkopotus izmaksu un lietojuma datus, pamatojoties uz jūsu nodrošināto vaicājumu. Izmantojot vaicājuma API, varat norādīt vēlamo filtrēšanu, kārtošanu un grupēšanu pēc visām pieejamajām dimensijām (piekļūstot no dimensiju API).

**Prognozētās izmaksas**

**Kāpēc izmaksu analīzē nav redzamas manu izmaksu prognozes?**  
Ir vairāki iemesli, kādēļ izmaksu analīzē trūkst prognozes prognožu, daži no tiem ir šādi:

1. Ja izmaksu dati ir mazāki par 10 dienām, prognozes diagramma netiks ielādēta. Lai modelī varētu izmantot precīzas projekcijas, ir nepieciešamas vismaz 10 dienas pēdējo izmaksu datu
2. Ja esat atlasījis vēsturiskos datumus, prognozes diagramma nebūs redzama. Lūdzu, atlasiet datumu diapazonu ar prognozes diagrammas nākotnes datumiem
3. Ja jūsu kontam ir vairākas valūtas, prognozes diagrammā tiks prognozētas tikai projekta izmaksas "Visas izmaksas USD"

**Kāpēc prognoze nemainās, veicot izmaiņas resursos?**  
Prognozes modelī ir nepieciešamas pāris dienas, lai ņemti vērā konta izmaiņas, un netiek veiktas tūlītējas projekcijas, ņemot vērā resursu izmaiņas  
Lielāku resursu palielināšanas vai samazināšanas darbību gadījumā modelī būs nepieciešams mazliet ilgāks laiks, lai pielāgotu šīs izmaiņas attiecībā uz anomālijām

**Kāpēc mana prognoze palielinās pēc tam, kad veicu rezervāciju vai Marketplace pirkumu?**  
Prognozes modelī tiek ņemti vērā jūsu "faktiskās izmaksas", un tas neattiecas uz lietojumu un iegādi atsevišķi. Ja iegādājaties vienreizēju pirkumu, pēc 10 dienām modelis samazinās projekcijas, ja pēkšņi palielināsies izmaksas

**Vēlos skatīt prognozes atsevišķai dimensijai (piemēram, Metrs)**  
Prognoze pašlaik atbalsta kopējo izmaksu projekcijas, nevis atsevišķus metriem. Tādējādi, ja dimensija tiek "grupēta pēc", projekcijas tiks prognozētas visu dimensijas elementu kopsummai.

**Ieteiktie dokumenti**

- [Kas ir Azure izmaksu pārvaldība?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure izmaksu pārvaldības paraugprakse](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Analizējiet savas izmaksas un izdevumus](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Izpētiet un analizējiet izmaksas, izmantojot izmaksu analīzi](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure izmaksu pārvaldība: cenas](https://azure.microsoft.com/services/cost-management/#pricing)
- [Pārskatīt izmaksas izmaksu analīzē](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Video apmācība: Budžeta izveide Azure portālā](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Budžeta skatīšanas un pielāgošanas priekšnosacījumi](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Budžetu izveide un pārvaldība](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Automatizācijas konfigurēšana, izmantojot Azure darbību grupas un budžeta API](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Brīdinājumu par izmaksām izmantošana, lai pārraudzītu lietojumu un izdevumus](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Izmaksu pārvaldības paraugprakse](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Apmācību video**

- [Budžeta izveide Azure portālā](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Pārvaldiet izmaksas, izmantojot budžeta API un darbību grupas](https://go.microsoft.com/fwlink/?linkid=2147038)