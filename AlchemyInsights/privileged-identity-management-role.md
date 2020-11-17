---
title: Priviliģētā identitātes pārvaldības loma
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
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088880"
---
# <a name="privileged-identity-managementpim-role"></a>Priviliģētā identitātes pārvaldības (PIM) loma

**Pēc lomas aktivizēšanas atļaujas nav piešķirtas**

Aktivizējot lomu Azure AD priviliģētā identitātes pārvaldībā (PIM), aktivizēšana var netikt uzreiz izplatīta visiem portāliem, kuriem nepieciešama privileģētā loma. Dažreiz pat tad, ja izmaiņas tiek izplatītas, tīmekļa kešatmiņa portālā var izraisīt izmaiņas, kas uzreiz neietekmēs.

Ja aktivizācija ir aizkavēta, veiciet tālāk norādītās darbības.

1. Izrakstieties no Azure portāla un pēc tam atkal pierakstieties. Aktivizējot Azure AD lomu vai Azure resursa lomu, redzēsit aktivizēšanas posmus. Kad visi posmi ir pabeigti, tiks parādīta saite Izrakstīties. Varat izmantot šo saiti, lai izrakstītos. Tas atrisinās lielāko daļu gadījumu aktivizēšanas atlikšanai.
2. Programmā PIM pārbaudiet, vai esat norādīts kā lomas dalībnieks.
3. Ja aktivizējat Exchange administratora lomu, noteikti izrakstieties un pierakstieties vēlreiz. Ja problēma joprojām pastāv, atveriet atbalsta biļeti un uzlabojiet to kā problēmu. Ja izmantojat Exchange administratora lomu, lai piekļūtu drošības un atbilstības centram, skatiet nākamo darbību.
4. Ja aktivizējat lomu, lai piekļūtu drošības un atbilstības centram, vai, ja aktivizējat SharePoint administratora lomu, jums būs zināma aktivizēšanas aizkave no dažām minūtēm līdz pat dažām stundām. Šī ir zināma problēma, un mēs aktīvi strādājam ar šīm grupām, lai atrisinātu šo problēmu pēc iespējas ātrāk.

Papildinformāciju skatiet rakstā:

- [Azure AD lomu aktivizēšana PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Azure resursu lomu aktivizēšana PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Atļaujas netiek noņemtas pēc lomas deaktivizēšanas vai lomas aktivizēšanas derīguma termiņa beigām**

Deaktivizējot lomu Azure AD privileģētā identitātes pārvaldībā vai pēc tam, kad beidzas lomas aktivizēšanas perioda termiņš, iespējams, ir aizkave, kur jums joprojām ir piekļuve.

Ja deaktivizēšana ir aizkavēta, veiciet tālāk norādītās darbības.

1. Ja aktivizējat Exchange administratora lomu vai lomas aktivizēšanas perioda beigas, un jūs nodarbina nozīmīgu atlikšanu pirms atļauju noņemšanas, atveriet atbalsta biļeti un informējiet savu atbalsta inženieri par to, lai palīdzētu jums iesniegt biļeti ar privileģētu piekļuves pārvaldības (PAM) grupu sistēmā Office par šo problēmu.
2. Ja aktivizēšanas periodam ir beidzies derīgums, bet joprojām ir atvērta pārlūka sesija, slēdziet pārlūkprogrammu. Jūs varat turpināt izmantot šo lomu, līdz aizvērsit šo sesiju. Šī ir zināma problēma, un mēs raugāmies uz iespējamu labojumu, lai aktīvi atsauktu katru sesiju, kad aktivizācija ir beigusies.

Ja kavējums ir atšķirīgs no šiem diviem scenārijiem, lūdzu, atveriet atbalsta biļeti.
