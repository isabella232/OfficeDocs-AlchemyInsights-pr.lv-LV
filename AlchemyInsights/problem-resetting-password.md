---
title: Problēma saistībā ar paroles atiestatīšanu
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
ms.openlocfilehash: 535b5273d367e24ac45b3f60dbc7b6a2da6a3d9affa5a67499989d19a1904768
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039973"
---
# <a name="problems-resetting-password"></a>Problēmas ar paroles atiestatīšanu

Tālāk ir norādītās dažas problēmas, ar kurām varat saskarties, atiestatot paroli, kā arī iespējamie risinājumi:

**Man radušās problēmas ar paroles atiestatīšanu, kas nav apskatīta citās kategorijās**

- Pārliecinieties, vai esat pilnvarots atiestatīt paroles. Tikai globālie, paroļu un lietotāju administratori var atiestatīt lietotāju paroles. Globālie administratori var arī atiestatīt citu priviliģētu administratoru paroles.
- Pārliecinieties, vai izprotat licencēšanas prasības:
    - Jūsu organizācijā ir jābūt piešķirtai vismaz vienai licencei.
        - Tikai mākoņa lietotāji — Office 365 (O365) maksas SKU vai Azure AD Basic
        - Mākonis un/vai lokālie lietotāji — Azure AD Premium P1 vai P2, Enterprise Mobility + Security (EMS) vai Secure Productive Enterprise (SPE)
        - Papildinformāciju par licencēšanas prasībām skatiet rakstā [Azure AD pašapkalpošanās paroles atiestatīšanas licencēšanas prasības.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)

**Man radušās problēmas ar iestatītās paroles atiestatīšanas politikas testēšanu**

- Nesen lietotās politikas var ilgt vairākas minūtes, lai replicētu visos datu centros un beigu punktos. Fiziskais attālums no datu centra ietekmēs arī to, cik ātri tiek lietotas izmaiņas.
- Testējam lietotāju, nevis administratoru, un pilots ar nelielu lietotāju kopu. Azure portālā konfigurētās politikas attiecas tikai uz lietotājiem, nevis administratoriem. Microsoft īsteno stipru noklusējuma divvārdu paroles atiestatīšanas politiku jebkurai Azure administratora lomai (piemērs: globālais administrators, palīdzības dienesta administrators, paroļu administrators utt.)
    - Uzziniet vairāk [par politikām administratoriem.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)

**Es vēlos izvietot paroles atiestatīšanu, bet nevēlos, lai lietotāji reģistrētu papildinformāciju par drošību**

Iepriekš aizpildiet datus saviem lietotājiem, lai tiem tie nebūtu jāaizpilda. — kā administrators varat saviem lietotājiem iestatīt tālruņa un e-pasta rekvizītus pirms paroles atiestatīšanas savā organizācijā. To var izdarīt, izmantojot API, PowerShell vai Azure AD Savienošana. Papildinformācija šeit:
- [Paroles atiestatīšanas izvietošana bez nepieciešamības lietotājiem reģistrēties](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Kādi dati tiek izmantoti, atiestatot paroli](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Paroles atiestatīšanas poga ir pelēkā krāsā**

Jūs neesat pilnvarots atiestatīt šī lietotāja paroles. Tikai globālie, paroļu un lietotāju administratori var atiestatīt lietotāju paroles. Globālie administratori var arī atiestatīt citu priviliģētu administratoru paroles.

**Es neredzu paroles atiestatīšanas asmeni**

Jūs neesat pilnvarots atiestatīt paroles. Tikai globālie, paroļu un lietotāju administratori var atiestatīt lietotāju paroles. Globālie administratori var arī atiestatīt citu priviliģētu administratoru paroles.

**Paroles atiestatīšanas laikā netiek parādīts lokālā integrācijas asmens disks**

- Lokālās integrācijas asmens redzams tikai hibrīdā vidē — tas nozīmē, ka izmantojat paroles atrisi, lai manipulētu ar lokālā lietotāja parolēm.
- Šis asmens stieps nav redzams, ja:
    - Jūs neizmantojat paroles rakstīšanasback
    - Radusies problēma ar paroles rakstīšanasback instalēšanu/savienojamību
    - Radusies problēma ar Azure AD Savienošana
    - Lai uzzinātu, kā novērst citas problēmas saistībā ar paroles atriti, skatiet sadaļu Paroles [rakstīšanas problēmu novēršana](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Es nezinu, kā atiestatīt lietotāja paroli**

1. Pierakstieties Azure portālā kā atbilstošs administrators.
1. Dodieties uz lietotāju un grupu asmens **sejiņu, atlasiet Visi lietotāji**.
1. Sarakstā atlasiet lietotāju.
1. Atlasītajam lietotājam atlasiet **Pārskats** un pēc tam komandjoslā noklikšķiniet uz **Atiestatīt paroli.**
1. Izpildiet ekrānā redzamos norādījumus.
    - Tiek atiestatītas tikai Azure portāla atbalsta paroles rakstīšanas laikā.

**Es atiestatu lokālā lietotāja paroli no Office 365 Admin portāla vai Office 365 lietojumprogrammas, bet lietotājs joprojām nevar pierakstīties**

Paroles rakstīšana šajā portālā netiek atbalstīta. Vēlreiz atiestatiet lietotāja paroli Azure portālā — portal.azure.com

