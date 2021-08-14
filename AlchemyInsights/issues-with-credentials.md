---
title: Problēmas ar akreditācijas datiem
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
- "9004330"
- "7723"
ms.openlocfilehash: 975d4850c1ecffae786dd19b7f4363e0c95378cff4f3ae6bb1968af33ef810b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986826"
---
# <a name="issues-with-credentials"></a>Problēmas ar akreditācijas datiem

[Microsoft indentitāšu platforma un OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) klienta akreditācijas datu plūsma apraksta, kā programma tiek tieši saistīta ar OAuth 2.0 klienta akreditācijas datu piešķires plūsmu.

**Kā pārvaldīt lietojumprogrammas paroles vai sertifikāta akreditācijas datus?**

Azure CLI varat izmantot [az reklāmas](https://docs.microsoft.com/cli/azure/ad/app/credential) programmu akreditācijas datus, lai dzēstu, uzskaitītu vai atiestatītu lietojumprogrammas paroles vai sertifikāta akreditācijas datus.

**Kā mani lietotāji atiestata paroles?**

Lietotājiem ir [jāreģistrējas pašapkalpošanās paroles atiestatīšanai,](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) lai viņi varētu atiestatīt savas paroles. Kad lietotājs ir reģistrējies, viņš var izpildīt šajā rakstā sniegtos norādījumus, lai atiestatītu paroli: [Darba vai mācību paroles atiestatīšana.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)

**Kā mani lietotāji maina paroles?**

Lietotāji var izpildīt šajā rakstā norādītās darbības, lai mainītu paroles: [Kā mainīt paroli.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)
Viņi var arī [pārvaldīt programmu paroles divsoļu pārbaudei.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)

**Mainot vai atiestatot paroli, mans lietotājs saņem kļūdu**

Šī saite sniegs informāciju par biežāk sastopamām problēmām, kas var rasties, ja lietotājs mēģina atiestatīt savu paroli: [Bieži sastopamās problēmas un to risinājumi](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Man rodas problēma, atiestatot lietotāja paroli**

- Pārliecinieties, vai esat pilnvarots atiestatīt paroles. *Tikai globālie, paroļu un lietotāju administratori var atiestatīt lietotāju paroles.* Globālie administratori var arī atiestatīt citu priviliģētu administratoru paroles.

- Pārliecinieties, vai izprotat licencēšanas prasības:

  - Jūsu organizācijā ir jābūt piešķirtai vismaz vienai licencei:
    - **Tikai mākoņa lietotāji** — Office 365 (O365) maksas SKU vai Azure AD Basic
    - **Mākonis un/vai** lokālie lietotāji — Azure AD Premium P1 vai P2, Enterprise Mobility + Security (EMS) vai Secure Productive Enterprise (SPE)
    - Papildinformāciju par licencēšanas prasībām skatiet [rakstā Azure AD pašapkalpošanās paroles atiestatīšanas licencēšanas prasības.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Lai atiestatītu lietotāja paroli, atrodiet lietotāju Azure AD. Pēc tam šī lietotāja pārskata asmens kartē noklikšķiniet uz pogas "atiestatīt paroli".

**Paroles atiestatīšanas poga ir pelēkā krāsā**

Jūs neesat **pilnvarots** atiestatīt šī lietotāja paroles. *Tikai globālie, paroļu un lietotāju administratori var atiestatīt lietotāju paroles.* Globālie administratori var arī atiestatīt citu priviliģētu administratoru paroles.

**Es neredzu paroles atiestatīšanas asmeni**

Jūs neesat pilnvarots atiestatīt paroles. *Tikai globālie, paroļu un lietotāju administratori var atiestatīt lietotāju paroles.* Globālie administratori var arī atiestatīt citu priviliģētu administratoru paroles.

**Paroles atiestatīšanas laikā netiek parādīts lokālā integrācijas asmens disks**

- Lokālās integrācijas asmens redzams tikai hibrīdā vidē — tas nozīmē, ka izmantojat paroles atrisi, lai manipulētu ar lokālā lietotāja parolēm.

- Šis asmens stieps nav redzams, ja:

  - Jūs neizmantojat paroles rakstīšanasback
  - Radusies problēma ar paroles rakstīšanasback instalēšanu/savienojamību
  - Radusies problēma ar Azure AD Savienošana
  - Lai uzzinātu, kā novērst citas problēmas saistībā ar paroles atriti, skatiet rakstu [Paroles rakstīšanasback problēmu novēršana](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Es nezinu, kā atiestatīt lietotāja paroli**

1. Pierakstieties Azure portālā kā atbilstošs administrators.
2. Dodieties uz **lietotāju un grupu asmens** sejiņu, **atlasiet Visi lietotāji**.
3. Sarakstā atlasiet lietotāju.
4. Atlasītajam lietotājam atlasiet **Pārskats** un pēc tam komandjoslā atlasiet **Atiestatīt paroli**.
5. Atlasiet pogu **Atiestatīt paroli** un izpildiet ekrānā redzamos norādījumus.
    - Tiek atiestatītas tikai Azure portāla **atbalsta paroles** rakstīšanas laikā.

**Es atiestatu lokālā lietotāja paroli no Office 365 Admin portāla vai Office 365 lietojumprogrammas, bet lietotājs joprojām nevar pierakstīties**

Paroles rakstīšana šajā portālā netiek atbalstīta. Vēlreiz atiestatiet lietotāja paroli Azure portālā.
