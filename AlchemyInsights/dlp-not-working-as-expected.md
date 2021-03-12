---
title: DLP nedarbojas, kā paredzēts
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707817"
---
# <a name="dlp-not-working-as-expected"></a>DLP nedarbojas, kā paredzēts

**Svarīgi**: šo bezprecedenta laiku mēs veicam darbības, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir plaši pieejami. Lai iegūtu papildinformāciju, apmeklējiet [SharePoint Online pagaidu līdzekļu pielāgojumi](https://aka.ms/ODSPAdjustments).

 **DLP iestatīšana**

Vai rodas problēmas ar **datu zuduma novēršanu (DLP)** sistēmā Office 365, nedarbojas, kā paredzēts? Ja jā, pārliecinieties, vai jūsu **DLP politika** ir iestatīta pareizi, un jūsu datos ir norādīts, kā tiek meklēta **DLP politika** , kad tas tiek novērtēts.
  
DLP politikas ļauj identificēt un aizsargāt sensitīvu informāciju jūsu organizācijā. Lai iestatītu DLP politikas, izmantojiet [šeit](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)esošo informāciju.
  
 **Ko DLP politikas meklē**
  
Izmantojot **iebūvētos sensitīvos informācijas tipus** drošības un atbilstības centros, DLP politikas meklē konkrētus modeļus un elementus, nosakot šos jutīgos tipus.
  
- **Iebūvētie sensitīvie informācijas tipi**

    Lai iegūtu informāciju par iebūvētajiem sensitīvajiem tipiem un to, kas ir paredzēts DLP politikai, nosakot sensitīvo tipu, skatiet rakstu: [kā izskatās sensitīvās informācijas tipi](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

- **Pielāgoti sensitīvie informācijas tipi**

    Ja mēģināt izveidot pielāgotus sensitīvos informācijas tipus, lai iegūtu informāciju par to, kā izveidot pielāgotu sensitīvu datu tipu, izmantojiet tālāk norādīto [rakstu.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)

**DLP politikas pārbaude**

Lai testētu savus datus ar iebūvētu vai pielāgotu sensitīvu informācijas tipu, izmantojiet opciju **testa veids** , kas pieejama sadaļā **klasificēti**  >  **sensitīvi informācijas tipi**. Papildinformāciju skatiet rakstā [pielāgotu sensitīvo informācijas tipu pārbaude](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).

 **Atskaites**
  
- Iegūstiet sensitīvus datus ieskatu ar [DLP atskaitēm.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Skatiet detalizētu informāciju par notikumu ar [starpgadījumu atskaiti](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).
