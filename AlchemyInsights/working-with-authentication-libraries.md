---
title: Darbs ar autentifikācijas bibliotēkām
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035828"
---
# <a name="working-with-authentication-libraries"></a>Darbs ar autentifikācijas bibliotēkām

Lai atrisinātu Microsoft autentifikācijas bibliotēkas (MSAL) problēmu, veiciet tālāk norādītās darbības.

1. **Darbs ar MSAL**: [Microsoft identitātes platformas autentifikācijas bibliotēkas](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) — šis raksts rāda Microsoft autentifikācijas bibliotēkas atbalstu vairākiem lietojumprogrammas tipiem. Tajā ir iekļautas saites uz bibliotēkas avota kodu; kur iegūt pakotnes lietojumprogrammas projektu. un vai bibliotēka atbalsta lietotāja pierakstīšanos (autentifikāciju), piekļuvi aizsargātajiem tīmekļa API (autorizācija) vai abiem.

2. **Autentifikācijas problēmu novēršana**: MSAL atbalsta vairākas autentifikācijas plūsmas, kas jāizmanto dažādos lietojumprogrammas scenārijos. Atkarībā no tā, kā jūsu klienta lietojumprogramma ir veidota, MSAL var izmantot vienu vai vairākas autentifikācijas plūsmas, ko atbalsta Microsoft Identity Platform. Šīs plūsmas var izveidot dažāda veida marķierus un autorizācijas kodus, kā arī pieprasīt atšķirīgas pilnvaras, lai tās darbotos.

3. **Piekļuves pilnvaras**: [Microsoft identitātes platformas piekļuves marķieri](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) — Uzziniet, kā jūsu API var validēt un izmantot prasības piekļuves pilnvarā. Visa šī raksta dokumentācija, izņemot gadījumus, kad tas ir norādīts, attiecas tikai uz pilnvarām, kas emitētas par jūsu reģistrēto API. Tas neattiecas uz pilnvarām, kas ir izsniegtas korporācijai Microsoft piederošiem API, un šīs pilnvaras nevar izmantot, lai validētu, kā Microsoft identitātes platforma izdos marķierus jūsu izveidotajam API.

**Azure Active Directory autentifikācijas bibliotēkas atbalsta beigas (ADAL)**

- **Sākot no 30. jūnija, 2020,** vairs nepievienosit nekādus jaunus līdzekļus, kas ADAL un Azure AD Graph. Mēs turpināsim nodrošināt tehnisko atbalstu un drošības atjauninājumus, bet vairs nenodrošināsim līdzekļu atjauninājumus.
- **Sākot no 30. jūnija, 2022,** mēs NODROŠINĀSIM atbalstu ADAL un Azure AD Graph un vairs nenodrošinās tehnisko atbalstu vai drošības atjauninājumus.
- Programmas, kas, izmantojot ADAL, pēc šī laika turpinās darboties, bet *nesaņem nekādu tehnisku atbalstu vai drošības atjauninājumus*.
- Lietojumprogrammas, kas izmanto Azure AD Graph pēc šī laika, iespējams, vairs nesaņems atbildes no Azure AD Graph galapunkta.

**PārADAL migrācija**

- Ieteicams atjaunināt uz MSAL, kurā ir jaunākie līdzekļi un drošības atjauninājumi.
- Ja izmantojat Microsoft apps, zināt, ka korporācija Microsoft turpina migrēt savas lietojumprogrammas uz MSAL pēc atbalsta termiņa beigām, nodrošinot, ka tās gūs labumu no MSAL pastāvīgajiem drošības un līdzekļu uzlabojumiem.

1. [Lasiet bieži uzdotos jautājumus par ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
2. [Uzziniet, kā migrēt programmas katrā platformā](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).
3. Ja pēc ceļveža izlasīšanas lietojumprogrammas platformā jums ir papildu jautājumi, varat publicēt [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) ar atzīmi [Azure-AD-ADAL-deprecat] vai atvērt problēmu bibliotēkas GitHub repozitorijā. **MSAL pārskata** raksta sadaļā [valodas un struktūras](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) skatiet saites uz katras bibliotēkas repo.
4. **Ja jums ir nepieciešama palīdzība, lai izprastu, kuras jūsu lietojumprogrammas izmanto ADAL**, iesakām pārskatīt visu programmas avota kodu. Ja nepieciešams, sazinieties ar visiem neatkarīgiem programmatūras piegādātājiem (ISV) vai lietojumprogrammu nodrošinātājiem. Microsoft atbalsta dienests var jums sniegt sarakstu ar visām jūsu nomniekā esošajām lietojumprogrammām, kas nav Microsoft ADAL lietojumprogrammas.







