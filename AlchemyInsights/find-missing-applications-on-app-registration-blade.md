---
title: Atrodiet trūkstošās lietojumprogrammas programmas reģistrācijas asmenī
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9654"
ms.openlocfilehash: 00b5821e2edad8b60ff60b1f85264d81c72277e4
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404697"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>Atrodiet trūkstošās lietojumprogrammas programmas reģistrācijas asmenī

1. Nevar atrast lietojumprogrammas lietojumprogrammu reģistrācijas portālā.

    Ja programma ir vairāku nomnieku programma un tā ir reģistrēta citā nomniekā, tā netiks rādīta zem programmas reģistrācijas asmens stūra. Tomēr pēc piekļuves (pēc piekrišanas) un jūsu nomniekā ir izveidota pakalpojuma pamatsumma, iespējams, to atradīsit Enterprise Applications asmens slāpī. Papildinformāciju skatiet rakstā [& identitātes platformas Azure AD — Microsoft identitātes platforma.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
2. Nevar skatīt programmas programmu reģistrācijas asmens slāpē, pat ja esat administrators.

    Pārliecinieties, vai esat pareizajā direktorijā Azure portālā.
3. Mana programma nav norādīta sadaļā Enterprise Applications asmens saraksts, bet tā tiek parādīta, kad es izveidoju vaicājumu PowerShell komandai.

    Dažreiz, kad lietojumprogrammu izdzēšat no Azure portāla, tā netiek rādīta portālā, bet, iespējams, nav pilnībā izdzēsta. Papildinformāciju skatiet šeit:
    - Varat izgūt iepriekš izdzēsto lietojumprogrammu sarakstu un redzēt, vai lietojumprogramma sarakstā tiek parādīta, izmantojot Powershell komandu: **Get-AzureADDeletedApplication**. Papildinformāciju skatiet rakstā [Get-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication)
    - Ja vēlaties pilnībā noņemt lietojumprogrammu, varat izmēģināt tālāk norādītos mēģinājumus programmā PowerShell: **Remove-AzureADApplication -ObjectId**. Papildinformāciju skatiet rakstā [AzureADApplication (AzureAD) noņemšana.](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication)
    - Vai arī varat mēģināt atjaunot izdzēsto lietojumprogrammu, izmantojot šādu Powershell komandu: **AzureADDeletedApplication -ObjectId** atjaunošana. Papildinformāciju skatiet rakstā [Restore-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
4. Savā jaunajā Azure nomniekā nevar atrast visu sākotnēji instalēto uzņēmuma lietojumprogrammu sarakstu.

    Pēc noklusējuma azure AD nav sākotnēji instalētas uzņēmuma lietojumprogrammas. Tā ir manuāli jāpievieno no opcijas "Jauna lietojumprogramma", pārlūkojot to no Azure AD galerijas vai pievienojot lietojumprogrammu, kas nav galerija. Papildinformāciju skatiet rakstā [Īsā pamācība: programmas pievienošana Azure Active Directory (Azure AD) nomniekam.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)
    Ja esat globālais administrators, varat viegli piekļūt savām programmām, izmantojot [Microsoft 365 lietojumprogrammu palaidēju](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher).
5. Nevar atrast manas lietojumprogrammas no portāla Manas lietojumprogrammas.

    Pārliecinieties, vai lietojumprogrammas nav paslēptas kolekcijas Mana lietojumprogramma lapā. Papildinformāciju skatiet rakstā [Kolekcijas (priekšskatījums) portālā Manas programmas — Azure AD.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections)
6. Lai startētu lietojumprogrammas no portāla Manas programmas, skatiet & programmu atrašana manu [lietojumprogrammu portālā — Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access).
7. Pēc instalēšanas Office 365 Mover programma netiek rādīta Enterprise Applications asmens slāpī.

    Lietojumprogramma "Office 365 Mover" ir vairāku nomnieku programma, kas nav jāpievieno AAD, izmantojot sadaļas Galerijas lietojumprogrammas sadaļā Enterprise Programmu reģistrācija. Lai piekļūtu Office 365 pārvietošanas programmai, vienkārši pierakstieties lietojumprogrammā un pieprasiet lietotāja piekrišanu atļaujām. Kad lietotājs būs sniedzis piekrišanu, šī lietojumprogramma tiks automātiski pievienota nomniekam ar e-pasta ID, kuru esat pieteicies.

    Pēc pierakstīšanās lietojumprogrammā jums jāspēj atrast šīs lietojumprogrammas ierakstu AAD sadaļā Enterprise Applications asmens lietojumprogrammu asmens. Lietojumprogramma ir jāmeklē, ierakstot vārdu un uzvārdu, piemēram, "Office 365 Mover" vai vienkārši meklējiet "office", un tajā jābūt uzskaitītai programmai. Lai uzzinātu vairāk, skatiet [rakstu Office 365 Mover](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)norāda, ka tas jau ir instalēts, bet nav norādīts Enterprise lietojumprogrammu galerijā.
8. Īsā pamācība: skatiet to lietojumprogrammu sarakstu, kuras izmanto jūsu [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) nomnieku identitātes pārvaldībai, parāda, kā skatīt lietojumprogrammas, kuras tiek dēvētas arī par lietojumprogrammām, kuras jau ir iestatītas izmantot jūsu Azure AD nomnieku kā identitātes nodrošinātāju (IdP).
9. [Novērsiet bieži sastopamās](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) problēmas, pievienojot vai noņemot lietojumprogrammu pakalpojumā Azure Active Directory, varat izprast biežāk sastopamās problēmas, ar kurām lietotāji saskaras ar lietojumprogrammu skatīšanu pakalpojumā Azure Active Directory.
