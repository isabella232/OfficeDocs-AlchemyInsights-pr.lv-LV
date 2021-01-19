---
title: Lietotāju problēmu novēršana
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
- "7813"
- "9004358"
ms.openlocfilehash: d9964e50bdea0c41ac14ab3783b579034b5f2c8c
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901041"
---
# <a name="announcements"></a>Paziņojumi

Sekojiet Google norādījumiem par saderību ar testēšanu, lai pārbaudītu, vai jūsu lietojumprogrammas ir ietekmētas. Google norādījumi ir pieejami https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support .

Pārliecinieties, vai, pierakstoties lietotājiem ar patērētāju Google kontiem, izmantojat sistēmas tīmekļa skatu vai sistēmas pārlūkprogrammu. Papildinformāciju skatiet rakstā problēmas, [pierakstoties lietojumprogrammā (-as), izmantojot tikai Chrome pārlūkprogrammu](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).


**Nevaru izveidot jaunu lietotāju savā Azure AD direktorijā**

Lai novērstu problēmu, ka Azure AD nav iespējams izveidot jaunu lietotāju, veiciet tālāk norādītās darbības.

1. Pārliecinieties, vai esat autorizēts izveidot jaunu standarta lietotāju. Azure Active Directory (AD) tikai globālā administratora vai lietotāja administratora loma var izveidot jaunu standarta lietotāju. Ja neesat kādā no šīm lomām, lūdziet administratoram pievienot jūs kādai no šīm lomām vai izveidot jaunu lietotāja kontu.
2. Pārliecinieties, vai lietotājvārds ir domēnā, kas ir verificēts Azure AD. Ja Azure AD nav pārbaudīti pielāgoti domēnu nosaukumi, varat izmantot Azure AD sākotnējo domēnu, kas beidzas ar *. onmicrosoft.com.
3. Pārliecinieties, vai lietotājvārds ir domēnā, kas nav Azure AD integrētās reklāmas no lokālās reklāmas. Lietotāji nevar pievienot mākonī ar domēnu nosaukumiem, kas tiek apvienoti no lokālās atrašanās vietas.
4. Pārliecinieties, vai nevienam lietotājam vai kontaktpersonai jau ir lietotājvārds, ko vēlaties piešķirt jaunajam lietotājam. Lietotāju nosaukumiem ir jābūt unikāliem visā Azure AD.
5. Skatiet [Azure AD lomas un administratorus](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) par savu Azure AD.
6. Skatiet Azure AD [domēnu nosaukumus](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Domains) .
7. Pārskatiet [audita žurnālus](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Audit) , lai skatītu detalizētāku informāciju par nesen izveidotu vai izdzēstu lietotāju, piemēram, kurš veica darbību, un kad.
8. Lai iegūtu papildinformāciju par jaunu lietotāju pievienošanu, skatiet sadaļu [debeszils portāla izmantošana, lai izveidotu jaunu lietotāju AZURE ad](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory) .
9. Lai iegūtu papildinformāciju par administratora lomu atļaujām Azure AD, skatiet rakstu [AZURE ad administratīvās lomas](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference).
10. Detalizētu informāciju par to, kā izveidot lietotāju, izmantojot Azure AD PowerShell, skatiet sadaļā [AZURE ad PowerShell, lai izveidotu jaunu lietotāju](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser).

**Problēma ar pašapkalpošanās reģistrēšanu**

Lai novērstu problēmas saistībā ar pašapkalpošanās reģistrēšanu, veiciet tālāk norādītās darbības.

1. Lai izmantotu patstāvīgi izmantojamas reģistrācijas lietojumprogrammas, vispirms ir jāiespējo patstāvīgi reģistrēties savam nomniekam. 
2. Lai iespējotu lietojumprogrammas atbalstu pašapkalpošanās reģistrēšanās, pievienojiet to lietotāja plūsmai. Nākamajā reizē, kad dosities uz šīs lietojumprogrammas pieteikšanās lapu, redzēsit opciju **_nav konta? Izveidojiet to!_* _. Tādējādi tiek sākts pašapkalpošanās reģistrācijas process.
3. Lai iegūtu informāciju par to, kā izmantot pašapkalpošanās reģistrēšanos, lai aizpildītu organizāciju Azure AD, skatiet rakstu [pašapkalpošanās reģistrācija pakalpojumam AZURE ad](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-self-service-signup).
4. Pēc tam, kad esat saistījis lietotāju plūsmu ar vienu vai vairākām lietojumprogrammām, lietotāji, kuri apmeklē šo programmu, varēs reģistrēties un iegūt viesa kontu, izmantojot lietotāja plūsmā konfigurētās opcijas. Lai iegūtu papildinformāciju par to, kā reģistrēt un iegūt viesa kontu, lietotāji var redzēt viesu lietotāju pašapkalpošanās [reģistrēšanu](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow).

*Kļūda, uzaicinot ārēju lietotāju**

Lai novērstu problēmas saistībā ar ārēja lietotāja uzaicināšanu, veiciet tālāk norādītās darbības.

Pārliecinieties, vai esat nosūtījis lietotāja uzaicinājumu uz e-pasta adresi, kas atbilst vārdam, ar kuru pierakstās lietotājs. Ja nosūtāt uzaicinājumu uz lietotāja starpniekservera e-pasta adresi, lietotājs to nevar izmantot. Papildinformāciju skatiet rakstā [AZURE ad B2B dokumentācija](https://docs.microsoft.com/azure/active-directory/external-identities/).

**Nevaru piešķirt licences lietotājam**

Lai novērstu problēmas saistībā ar licenču piešķiršanu lietotājam, veiciet tālāk norādītās darbības.

1. Lai pārvaldītu lietotāju licences, pārliecinieties, vai izmantojat kontu ar vienu no nepieciešamajām administratora lomām: globālais administrators, licenču administrators vai lietotāja administrators. Varat pārbaudīt lietotāja lomu lietotāja diska cilnē **direktorija loma** .
2. Ja izmantojat Azure portālu un licenču piešķiršana neizdodas, noklikšķiniet uz paziņojuma augšējā labajā stūrī. Tiks atvērts asmens ar detalizētu informāciju par to, kas notika nepareizi. Lielākajā daļā gadījumu tas ir pietiekami, lai saprastu un atrisinātu problēmu.
3. Lai lietotājam varētu piešķirt licenci, pārliecinieties, vai ir iestatīts lietotāja rekvizīts **lietojuma vieta** . Pārbaudiet, vai lietotājam ir šī rekvizīta kopa, skatot lietotāja asmens cilni **profils** .
4. Pārliecinieties, vai ir pieejamas pietiekamas licences produktam, kuru mēģināt piešķirt. Pieejamo licenču skaitu Azure portālā varat skatīt Azure [Active Directory-> licences-> visiem produktiem](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/LicensesMenuBlade/Products).
5. Lietotājam, iespējams, jau ir cita licence, kuras pakalpojumi konfliktē ar jaunajām licencēm, ko mēģināt piešķirt. Piemēram, ja lietotājam ir iespējots pakalpojums Exchange Online (1. plāns), jūs nevarēsit piešķirt licenci pakalpojumam Exchange Online (2. plāns). Atspējojiet kādu no pakalpojumiem, lai atļautu jauno licenču piešķiršanu. Ja izmantojat Azure Portal vai PowerShell cmdlet, **detalizētās informācijas** lapā ir uzskaitīti īpašie pakalpojumi, kas izraisa konfliktu.
6. Ja mēģināt noņemt licenci un tas neizdodas, lietotājam var būt citas licences ar pakalpojumiem, kas ir atkarīgi no pakalpojumiem, kurus cenšaties noņemt. Ja izmantojat Azure Portal vai PowerShell cmdlet, kļūdas ziņojumā tiek uzskaitīti konkrēti pakalpojumi, kuriem ir atkarības.
7. Ja vēlaties saprast, kāpēc no lietotāja ir pievienota vai noņemta licence (piemēram, kurš vēl jūsu organizācijā ir veicis izmaiņas), pārbaudiet audita žurnālus. Iestatiet filtru, lai tiktu rādītas visas modifikācijas, ieskaitot tās **, kas tās** ir veikušas.
8. Ja izmantojat Exchange Online, daži nomnieka lietotāji, iespējams, ir nepareizi konfigurēti ar to pašu starpniekservera adreses vērtību. Šādos gadījumos, iespējams, redzēsit vispārējus kļūdu ziņojumus, ja licences operācija bankrotē. [Šajā rakstā](https://docs.microsoft.com/exchange/troubleshoot/administration/proxy-address-being-used) ir sniegta papildinformācija par šo problēmu, tostarp informācija par to, [kā izveidot savienojumu ar Exchange Online, izmantojot Remote PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell). Lai noteiktu, kuri lietotāji jūsu nomniekā satur to pašu starpniekservera adresi, izpildīs šo Exchange Online cmdlet:

Palaist

Get-Recipient | kur {$ _. Parametrā EmailAddresses norādītā-Match <user principal name> } | fL nosaukums, RecipientType, parametrā EmailAddresses norādītā





