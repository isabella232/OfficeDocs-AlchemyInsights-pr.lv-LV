---
title: Problēmas atiestatot paroli
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694379"
---
# <a name="problems-resetting-password"></a>Problēmas atiestatot paroli

Tālāk norādītas dažas problēmas, kas var rasties, atiestatot paroli un iespējamos risinājumus:

**Man ir problēma ar paroles atiestatīšanu, kas nav iekļauta citās kategorijās**

- Pārliecinieties, vai jums ir atļauts Atiestatīt paroles. Tikai globālie, paroļu un lietotāju administratori var atiestatīt lietotāju paroles. Globālie administratori var arī atiestatīt citas privilēģijas administratora paroles.
- Pārliecinieties, vai jums ir izpratne par licencēšanas prasībām:
    - Jums ir nepieciešama vismaz viena licence, kas piešķirta jūsu organizācijā
        - Tikai mākoņi — visi Office 365 (O365) apmaksātie SKU vai Azure AD Basic
        - Mākoņa un/vai Lokālie lietotāji — Azure AD Premium P1 vai P2, Enterprise Mobility + Security (EMS) vai Secure ražīgs uzņēmums (SPE)
        - Papildinformāciju par licencēšanas prasībām skatiet rakstā Azure AD pašapkalpošanās [paroles atiestatīšanas licencēšanas prasības](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).

**Man ir problēmas ar iestatītās paroles atiestatīšanas politikas testēšanu**

- Nesen lietotās politikas var ilgt vairākas minūtes, lai tās atdarinātu visos datu centros un galapunktos. Arī fiziskais attālums no datu centra ietekmēs, cik ātri izmaiņas tiek lietotas.
- Testējiet ar lietotāju, nevis administratoru un pilots ar nelielu lietotāju kopu. Azure portālā konfigurētās politikas attiecas tikai uz lietotājiem, nevis administratoriem. Microsoft ievieš spēcīgu noklusējuma divu vārtu paroles atiestatīšanas politiku jebkurai Azure administratora lomai (piemēram: globālā administratora, palīdzības dienesta administrators, paroļu administrators utt.)
    - Uzziniet vairāk par [administratoru politikām](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).

**Es vēlos izvietot paroles atiestatīšanu, bet nevēlos, lai lietotāji reģistrētu papildu drošības informāciju**

Iepriekš aizpildiet datus saviem lietotājiem, lai tiem nebūtu! -Kā administrators varat iestatīt tālruņa un e-pasta rekvizītus saviem lietotājiem, pirms izlaižat paroles atiestatīšanu savai organizācijai. To var izdarīt, izmantojot API, PowerShell vai Azure AD Connect. Papildinformācija šeit:
- [Paroles atiestatīšanas izvietošana bez nepieciešamības lietotājiem reģistrēties](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Kādus datus izmanto paroles atiestatīšana](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Paroles atiestatīšanas poga ir pelēkota**

Jūs neesat autorizēts šī lietotāja paroļu atiestatīšanai. Tikai globālie, paroļu un lietotāju administratori var atiestatīt lietotāju paroles. Globālie administratori var arī atiestatīt citas privilēģijas administratora paroles.

**Nav redzams paroles atiestatīšanas asmens**

Jūs neesat autorizēts, lai atiestatītu paroles. Tikai globālie, paroļu un lietotāju administratori var atiestatīt lietotāju paroles. Globālie administratori var arī atiestatīt citas privilēģijas administratora paroles.

**Paroles atiestatīšana nav redzama lokālā integrācijas asmens**

- Lokālā integrācijas asmens tiek rādīts tikai hibrīdās vidēs — tas nozīmē, ka izmantojat paroļu arī atpakaļrakstīšanas, lai manipulētu ar lokālo lietotāju parolēm.
- Šis asmens nav redzams, ja:
    - Jūs neizmantojat paroļu arī atpakaļrakstīšanas
    - Ir radusies problēma ar jūsu paroļu arī atpakaļrakstīšanas instalāciju/savienojamību
    - Ir radusies problēma ar Azure AD Connect instalēšanu/savienojamību
    - Papildinformāciju par problēmu novēršanu saistībā ar paroļu arī atpakaļrakstīšanas skatiet sadaļā [problēmu novēršana paroļu arī atpakaļrakstīšanas](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Es nezinu, kā atiestatīt lietotāja paroli**

1. Pierakstieties Azure portālā kā atbilstošs administrators.
1. Dodieties uz lapu lietotāji un grupas, atlasiet **Visi lietotāji**.
1. Sarakstā atlasiet lietotāju.
1. Atlasītajam lietotājam atlasiet **pārskats** un pēc tam komandjoslā noklikšķiniet uz **Atiestatīt paroli**.
1. Izpildiet ekrānā redzamos norādījumus.
    - Tiek atiestatīta tikai Azure portāla atbalsta paroles arī atpakaļrakstīšanas.

**Atjaunoju lokālā lietotāja paroli no Office 365 administrēšanas portāla vai Office 365 mobilās lietojumprogrammas, taču lietotājs joprojām nevar pierakstīties**

Paroļu arī atpakaļrakstīšanas šajā portālā netiek atbalstīts. Vēlreiz atiestatiet lietotāja paroli Azure portālā-portal.azure.com

