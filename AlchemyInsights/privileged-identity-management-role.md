---
title: Privileged Identity Management loma
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
- "9003230"
- "6825"
ms.openlocfilehash: 358e446192e6b58ace81afa06e0d65ae3a207282351ffc3ec9975a24779951fb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973236"
---
# <a name="privileged-identity-managementpim-role"></a>Privileged Identity Management(PIM) loma

**Atļaujas netiek piešķirtas pēc lomas aktivizēšanas**

Aktivizējot lomu Azure AD Privileged Identity Management (PIM), aktivizēšana var ne uzreiz tikt izplatīta visos portālās, kam ir nepieciešama priviliģētā loma. Dažreiz pat tad, ja izmaiņas tiek izplatītas, tīmekļa kešatmiņa portālā var neīst izmaiņas uzreiz.

Ja jūsu aktivizācija tiek aizkavēta, veiciet tālāk norādītās darbības.

1. Izrakstieties no Azure portāla un pēc tam pierakstieties atpakaļ. Aktivizējot Azure AD lomu vai Azure resursa lomu, redzēsit aktivizācijas posmus. Kad visi posmi būs pabeigti, būs redzama saite Izrakstīties. Varat izmantot šo saiti, lai izrakstītos. Šādi tiks atrisināta lielākā daļa aktivizācijas aizkaves gadījumu.
2. Lodziņā PIM pārbaudiet, vai esat norādīts kā lomas dalībnieks.
3. Ja aktivizējot administratora Exchange, pārliecinieties, vai izrakstāties un atkal pierakstāties. Ja problēma joprojām pastāv, atveriet atbalsta biļeti un paceliet to kā problēmu. Ja izmantojat savu Exchange administratora lomu, lai piekļūtu drošības un atbilstības centram, skatiet nākamo darbību.
4. Ja aktivizējot lomu, lai piekļūtu drošības un atbilstības centram vai aktivizējot SharePoint administratora lomu, dažas minūtes līdz dažām stundām aizkavēsiet jūs. Šī ir zināma problēma, un mēs aktīvi sadarbojamies ar šīm grupām, lai pēc iespējas drīzāk atrisinātu šo problēmu.

Papildinformāciju skatiet rakstā:

- [Azure AD lomu aktivizēšana PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Azure resursu lomu aktivizēšana PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Atļaujas netiek noņemtas pēc lomas deaktivizēšanas vai beidzas lomas aktivizēšanas derīgums**

Deaktivizējot lomu Azure AD Privileged Identity Management vai kad beidzas lomas aktivizēšanas periods, iespējams, aizkave, kur joprojām varat piekļūt.

Ja jūsu deaktivizēšana tiek aizkavēta, veiciet tālāk norādītās darbības.

1. Ja deaktivizējat Exchange administratora lomu vai beidzas lomas aktivizēšanas periods un pamanāt būtisku aizkavi pirms atļauju noņemšanas, atveriet atbalsta biļeti un informējiet atbalsta speciālistu par darbu ar priviliģētās piekļuves pārvaldības (Privileged Access Management — PAM) grupu programmā Office par šo problēmu.
2. Ja aktivizācijas periods ir beidzies, bet joprojām ir atvērta pārlūkprogrammas sesija, aizveriet pārlūkprogrammu. Lomu varat turpināt izmantot līdz brīdim, kad slēdzat šo sesiju. Šī ir zināma problēma, un mēs meklējam iespējamo labojumu, kas var aktīvi atsaukt katru sesiju, kad ir beidzies aktivizācijas derīgums.

Ja aizkave atšķiras no šiem diviem scenārijiem, lūdzu, atveriet atbalsta biļeti.
