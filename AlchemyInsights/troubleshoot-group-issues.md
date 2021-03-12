---
title: Grupas problēmu novēršana
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7814"
- "9004358"
ms.openlocfilehash: 7e2957a27305e8fb0bfd10e21189cef9870c5aaa
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/18/2021
ms.locfileid: "50714053"
---
# <a name="troubleshoot-group-issues"></a>Grupas problēmu novēršana

**Man ir jāpiešķir grupa Azure AD lomai**

Lai piešķirtu Azure Active Directory (AD) grupu Azure AD lomai, veiciet tālāk norādītās darbības.

1. Izveidot jaunu grupu — lai izveidotu jaunu grupu:

    izveide. Pierakstieties Azure AD administrēšanas centrā ar privileģētās lomas administratoru vai globālā administratora atļaujām. 
    b. Atlasiet Azure Active Directory > grupas > visas grupas > jauna grupa. 
    c. Izveidot grupu.

2. Piešķiriet lomu grupai grupas izveides laikā vai pēc tam, kad grupa ir izveidota.

    izveide. Lai piešķirtu grupai lomu grupas izveides laikā, pārslēdzieties uz pārslēgšanas Azure AD lomām var piešķirt grupai un izveidot grupu.
    b. Lai piešķirtu lomu grupai pēc tās izveides, pārejiet uz jaunizveidotās grupas cilni piešķirtās lomas un piešķiriet lomai grupu.

**Man ir nepieciešama, lai pārvaldītu Azure AD lomai piešķirtās grupas dalību**

1. Lai izvairītos no privilēģiju palielināšanas, pēc noklusējuma tikai priviliģētās lomas administrators un globālais administrators var modificēt lomai piešķirtās grupas dalību. Tomēr viņi var izvēlēties piešķirt šīs grupas īpašnieku un deleģēt šo uzdevumu. Papildinformāciju skatiet sadaļā [mākoņa grupu izmantošana, lai pārvaldītu lomu piešķires Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).
2. Bieži uzdotie jautājumi un problēmu novēršanas padomi par lomu piešķiršanu grupām Azure AD, skatiet rakstā [Cloud groups piešķirto lomu problēmu novēršana](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).

**Dinamiskās grupas**

1. Ja nevarat atrast iebūvētos lietotāja atribūtus, nodrošiniet, lai atribūts būtu atbalstīto rekvizītu sarakstā.
2. Ja meklējat iebūvētu ierīces atribūtu, pārliecinieties, vai atribūts ir ierīču atribūtu sarakstā 
3. Papildus iebūvētajiem lietotāja un ierīces atribūtiem varat izmantot arī [paplašinājuma atribūtus](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties). Pēc paplašinājuma atribūtu sinhronizēšanas no lokālās Windows Server AD vai pievienotas SaaS lietojumprogrammas, atribūtiem jābūt redzamiem kārtulu veidotāja nolaižamajā sarakstā. Pielāgotā atribūta nosaukumu var atrast direktorijā, veicot vaicājumu lietotāja atribūtam, izmantojot PowerShell un meklējot atribūta nosaukumu. Tos var izmantot arī, veidojot kārtulas sintakses kārtulās.
4. Pārliecinieties, vai nomniekam ir attiecīgā licence. Dinamiskām grupām nepieciešams, lai nomniekam būtu Azure AD P1 Premium licence. Azure AD licenču plānu sarakstam var piekļūt [šeit](https://azure.microsoft.com/pricing/details/active-directory/). Enterprise Mobility + drošības licencēšanas plāniem var piekļūt [šeit](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing).
5. Pārliecinieties, vai lietotāja, kas veido dinamisko grupu, loma ir globālais administrators, Intune administrators, grupas administrators vai lietotāja administrators.
6. Lūdzu, atļaujiet grupas laiku aizpildīt. Atkarībā no nomnieka lieluma grupai var paiet līdz pat 24 stundām, lai to aizpildītu pirmoreiz vai pēc kārtulas izmaiņām.
7. Papildinformāciju skatiet rakstā [uz atribūtu balstītas kārtulas izveide dinamiskās grupas dalībai](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership).

**Grupai ir jāizdzēš**

1. Grupas var izdzēst no direktorija, izmantojot Remove-AzureADGroup cmdlet Azure AD PowerShell modulī.
2. Pirms mēģināt dzēst sinhronizētu grupu Azure AD, pārliecinieties, vai esat izdzēsis visas piešķirtās licences, lai novērstu kļūdas.
3. Papildinformāciju par grupu dzēšanu skatiet rakstā [grupas dzēšana ar piešķirtu licenci](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license).

**Ir jāatjauno izdzēsta grupa**

1. Ja Office 365 grupa ir izdzēsta, tā var tikt atjaunota tikai līdz 30 dienām, līdz tiek veikta neatgriezeniska dzēšana. Pēc tam, kad tā ir neatgriezeniski izdzēsta, grupu vairs nevar atjaunot. Uzziniet vairāk par grupu atjaunošanu [šeit](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).
2. Šī funkcionalitāte netiek atbalstīta drošības grupām un adresātu grupām.
3. Pārliecinieties, vai jums ir atļauja atjaunot Office 365 grupu. Globālie administratori, grupu Administratori, lietotāju kontu administratori, Intune pakalpojumu administratori, partneru 1. pakāpes vai 2. pakāpes atbalsts un grupas īpašnieks var atjaunot grupu.
4. Kad dinamiskā grupa ir izdzēsta un atjaunota, tā tiek uzskatīta par jaunu grupu un atkārtoti aizpildīta atbilstoši kārtulai. Šis process var ilgt līdz pat 24 stundām.
5. Papildinformāciju par izdzēstas grupas atjaunošanu skatiet rakstā [izdzēstas Office 365 grupas atjaunošana Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Grupas termiņa politikas konfigurācija**

1. Šī funkcionalitāte tiek atbalstīta tikai Office 365 grupām, nevis drošības grupām un adresātu grupām netiek atbalstītas.
2. Office 365 grupu derīguma politikas konfigurēšana un lietošana prasa Azure AD Premium licenci.
3. Pašlaik tikai vienu termiņa politiku var konfigurēt Office 365 grupām nomniekā.
4. Grupu var atjaunot tikai globālie administratori, grupu Administratori, lietotāju administratori un grupas īpašnieks.
5. Ja Office 365 grupai ir beidzies derīgums, tas tiek izdzēsts, un to var atjaunot tikai līdz 30 dienām, pirms tiek veikta pastāvīga dzēšana. Pēc tam, kad tā ir neatgriezeniski izdzēsta, grupu vairs nevar atjaunot. Uzziniet vairāk par grupu atjaunošanu [šeit](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Uz darbību pamatota automātiskā atjaunošana**

SharePoint, Outlook un Teams lietotāju darbības var izraisīt grupas automātisko atjaunošanu. Darbības tiek pārbaudītas 35 dienās, pirms beidzas grupas derīgums. Ja pašreizējā grupas dzīves cikla laikā ir aktivitāte, grupa tiks automātiski atjaunota un e-pasta paziņojums netiks nosūtīts grupu īpašniekiem.

**Paziņojumu hronometrāža noilgušām grupām**

1. E-pasta paziņojumi tiek nosūtīti Office 365 grupas īpašniekiem 30 dienas, 15 dienas un 1 dienu pirms grupas beigām.
2. Pirmoreiz iestatot derīguma termiņu, visas grupas, kas ir vecākas par derīguma periodu, tiek iestatītas uz 35 dienām līdz termiņa beigām.
3. Grupas derīguma beigu datums tiek aprēķināts, pamatojoties uz grupas atjaunošanas datumu, kas nav pamatots uz politikas atjaunināšanas datumu. Ja tiek atjaunināta termiņa politika, derīguma beigu datums nemainīsies.
4. Lai iegūtu papildinformāciju, skatiet rakstu [grupu termiņu politika un atjaunošanas e-pasta ziņojumi](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) un [atjaunot izdzēsto Office 365 grupu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Atļauja izveidot grupu**

Pārliecinieties, vai esat autorizēts izveidot jaunu grupu. Globālie administratori var atspējot grupu izveidi Azure portālā vai piekļuves panelī. Iespējams, ka jums ir nepieciešams administrators, lai izveidotu jaunu grupu vai piešķirtu atbilstošas atļaujas.

1. [Jaunas grupas izveide un dalībnieku pievienošana Azure portālā](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [Grupu izveide PowerShell MSOnline](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [Grupu izveides atspējošana PowerShell](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [To personu pārvaldība, kuras var izveidot grupas pakalpojumā Office 365](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. [Office 365 sveiciena paziņojuma atspējošana, izmantojot PowerShell](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. [Azure AD administrēšanas lomas](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

**Grupu izveides atļauju pārvaldība**

1. Globālie administratori var pārvaldīt grupas izveides atļaujas drošības vai Office 365 Groups, kas izveidotas Azure portālā vai piekļuves panelī, iestatot **lietotāji var izveidot drošības grupas Azure portāliem** vai **lietotājiem var izveidot Office 365 grupas Azure portālu** iestatījumos **visās grupās > Vispārīgi (iestatījumi)**.
2. Varat arī ierobežot grupu izveidi, lai atlasītu lietotāju grupu, ja jums ir Azure AD P1 Premium licence.

**Sveiciena paziņojuma atspējošana jauniem Office 365 grupas dalībniekiem**

Sveiciena paziņojumu, kas nosūtīts lietotājiem, kuri tiek pievienoti Office 365 grupām, var atspējot, iestatot `UnifiedGroupWelcomeMessageEnabled` uz **aplams** programmā PowerShell. Uzziniet par šo iestatījumu [šeit](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup).













