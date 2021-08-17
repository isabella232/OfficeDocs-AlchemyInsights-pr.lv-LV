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
ms.openlocfilehash: 0dee7e44a8701e1df924b9657cce6cf9d90160e58277d667f6069a4cbcf87ce5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057109"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>Atrodiet trūkstošās lietojumprogrammas programmas reģistrācijas asmenī

1. Nevar atrast lietojumprogrammas lietojumprogrammu reģistrācijas portālā.

    Ja programma ir vairāku nomnieku programma un tā ir reģistrēta citā nomniekā, tā netiks rādīta zem programmas reģistrācijas asmens stūra. Tomēr pēc piekļuves (pēc piekrišanas) un jūsu nomniekā ir izveidota pakalpojuma pamatsumma, iespējams, to atradīsit Enterprise Applications asmens slāpī. Papildinformāciju skatiet rakstā [Lietojumprogrammas & pamatnosaukumi pakalpojumā Azure AD — Microsoft indentitāšu platforma.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
2. Nevar skatīt programmas programmu reģistrācijas asmens slāpē, pat ja esat administrators.

    Pārliecinieties, vai esat pareizajā direktorijā Azure portālā.
3. Mana programma nav norādīta sadaļā Enterprise Applications asmens saraksts, bet tā tiek parādīta, kad es izveidoju vaicājumu PowerShell komandai.

    Dažreiz, kad lietojumprogrammu izdzēšat no Azure portāla, tā netiek rādīta portālā, bet, iespējams, nav pilnībā izdzēsta. Papildinformāciju skatiet rakstā:
    - Varat izgūt iepriekš izdzēsto lietojumprogrammu sarakstu un redzēt, vai lietojumprogramma sarakstā tiek parādīta, izmantojot Powershell komandu: **Get-AzureADDeletedApplication**. Papildinformāciju skatiet rakstā [Get-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication)
    - Ja vēlaties pilnībā noņemt lietojumprogrammu, varat izmēģināt tālāk norādītos mēģinājumus programmā PowerShell: **Remove-AzureADApplication -ObjectId**. Papildinformāciju skatiet rakstā [AzureADApplication (AzureAD) noņemšana.](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication)
    - Vai arī varat mēģināt atjaunot izdzēsto lietojumprogrammu, izmantojot šādu Powershell komandu: **AzureADDeletedApplication -ObjectId** atjaunošana. Papildinformāciju skatiet rakstā [Restore-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
4. Savā jaunajā Azure nomniekā nevar atrast visu sākotnēji instalēto uzņēmuma lietojumprogrammu sarakstu.

    Pēc noklusējuma azure AD nav sākotnēji instalētas uzņēmuma lietojumprogrammas. Tā ir manuāli jāpievieno no opcijas "Jauna lietojumprogramma", pārlūkojot to no Azure AD galerijas vai pievienojot lietojumprogrammu, kas nav galerija. Papildinformāciju skatiet rakstā [Īsā pamācība: lietojumprogrammas pievienošana Azure Active Directory (Azure AD) nomniekam.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)
    Ja esat globālais administrators, varat viegli piekļūt savām lietojumprogrammām, izmantojot [Microsoft 365 palaidēju](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher).
5. Nevar atrast manas lietojumprogrammas no portāla Manas lietojumprogrammas.

    Pārliecinieties, vai lietojumprogrammas nav paslēptas kolekcijas Mana lietojumprogramma lapā. Papildinformāciju skatiet rakstā [Kolekcijas (priekšskatījums) portālā Manas programmas — Azure AD.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections)
6. Lai startētu lietojumprogrammas no portāla Manas programmas, skatiet & programmu atrašana manu [lietojumprogrammu portālā — Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access).
7. Office 365 Mover programma pēc instalēšanas netiek rādīta Enterprise Applications asmens slāpēšanas vietā.

    Lietojumprogramma Office 365 Mover ir vairāku nomnieku programma, kas nav jāpievieno AAD, izmantojot sadaļas Galerijas lietojumprogrammas sadaļā Uzņēmuma programmu reģistrācija. Lai Office 365 programmu Mover, vienkārši pierakstieties lietojumprogrammā un pieprasiet lietotāja piekrišanu atļaujām. Kad lietotājs būs sniedzis piekrišanu, šī lietojumprogramma tiks automātiski pievienota nomniekam ar e-pasta ID, kuru esat pieteicies.

    Pēc pierakstīšanās lietojumprogrammā jums jāspēj atrast šīs lietojumprogrammas ierakstu AAD sadaļā Enterprise Applications asmens lietojumprogrammu asmens. Lietojumprogramma ir jāmeklē, ierakstot vārdu un uzvārdu, piemēram, "Office 365 Mover" vai vienkārši meklējiet "office", un tā var uzskaitīt lietojumprogrammu. Papildinformāciju skatiet rakstā Office 365 Mover norāda, ka tā jau ir instalēta, bet nav [iekļauta Enterprise lietojumprogrammu galerijā.](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)
8. Īsā pamācība: skatiet to lietojumprogrammu sarakstu, kuras izmanto jūsu [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) nomnieku identitātes pārvaldībai, parāda, kā skatīt lietojumprogrammas, kuras tiek dēvētas arī par lietojumprogrammām, kuras jau ir iestatītas izmantot jūsu Azure AD nomnieku kā identitātes nodrošinātāju (IdP).
9. [Novērsiet bieži sastopamās problēmas,](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) pievienojot vai noņemot lietojumprogrammu pakalpojumā Azure Active Directory izprast bieži sastopamās problēmas, ar kurām lietotāji saskaras ar lietojumprogrammu skatīšanu Azure Active Directory.
