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
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063680"
---
# <a name="issues-with-credentials"></a>Problēmas ar akreditācijas datiem

[Microsoft identitātes platformā un oauth 2,0 klienta akreditācijas datu plūsmā](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) ir paskaidrots, kā programmēt tieši atbilstoši OAuth 2,0 klienta akreditācijas datu plūsmai.

**Kā pārvaldīt lietojumprogrammas paroles vai sertifikāta akreditācijas datus?**

Azure CLI varat izmantot [AZ ad lietojumprogrammas akreditācijas](https://docs.microsoft.com/cli/azure/ad/app/credential) datus, lai izdzēstu, sarakstu vai atiestatītu lietojumprogrammas paroles vai sertifikāta akreditācijas datus.

**Kā mani lietotāji var atiestatīt savas paroles?**

Lai varētu atiestatīt savas paroles, lietotājiem ir [jāreģistrējas pašapkalpošanās paroles atiestatīšanai](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) . Pēc tam, kad lietotājs ir reģistrējies, viņš var izpildīt šajā rakstā sniegtos norādījumus, lai atiestatītu paroli: [darba vai skolas paroles](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)atiestatīšana.

**Kā mani lietotāji var mainīt savas paroles?**

Lietotāji var veikt šajā rakstā norādītās darbības, lai mainītu paroles: [kā mainīt paroli](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).
Tās var arī [pārvaldīt programmu paroles divsoļu pārbaudei](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).

**Mainot vai atiestatot paroli, mans lietotājs saņem kļūdas ziņojumu**

Šajā saitē būs sniegta informācija par bieži sastopamām problēmām, kas var rasties, ja lietotājs mēģina atiestatīt paroli: [biežāk sastopamās problēmas un to risinājumi](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Man radās problēma, atiestatot lietotāja paroli**

- Pārliecinieties, vai jums ir atļauts Atiestatīt paroles. *Tikai globālie, paroļu un lietotāju administratori var atiestatīt lietotāju paroles.* Globālie administratori var arī atiestatīt citas privilēģijas administratora paroles.

- Pārliecinieties, vai jums ir izpratne par licencēšanas prasībām:

  - Jums ir jābūt vismaz vienai jūsu organizācijā piešķirtai licencei:
    - **Tikai mākoņi** — visi Office 365 (O365) apmaksātie SKU vai Azure AD Basic
    - **Mākoņa un/vai Lokālie lietotāji** — Azure AD Premium P1 vai P2, Enterprise Mobility + Security (EMS) vai Secure ražīgs uzņēmums (SPE)
    - Papildinformāciju par licencēšanas prasībām skatiet rakstā Azure AD pašapkalpošanās [paroles atiestatīšanas licencēšanas prasības](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).
- Lai atiestatītu lietotāja paroli, atrodiet lietotāju Azure AD. Pēc tam šī lietotāja apskata asmenī noklikšķiniet uz pogas "Atiestatīt paroli".

**Paroles atiestatīšanas poga ir pelēkota**

Jūs neesat autorizēts **Šī** lietotāja paroļu atiestatīšanai. *Tikai globālie, paroļu un lietotāju administratori var atiestatīt lietotāju paroles.* Globālie administratori var arī atiestatīt citas privilēģijas administratora paroles.

**Nav redzams paroles atiestatīšanas asmens**

Jūs neesat autorizēts, lai atiestatītu paroles. *Tikai globālie, paroļu un lietotāju administratori var atiestatīt lietotāju paroles.* Globālie administratori var arī atiestatīt citas privilēģijas administratora paroles.

**Paroles atiestatīšana nav redzama lokālā integrācijas asmens**

- Lokālā integrācijas asmens tiek rādīts tikai hibrīdās vidēs — tas nozīmē, ka izmantojat paroļu arī atpakaļrakstīšanas, lai manipulētu ar lokālo lietotāju parolēm.

- Šis asmens nav redzams, ja:

  - Jūs neizmantojat paroļu arī atpakaļrakstīšanas
  - Ir radusies problēma ar jūsu paroļu arī atpakaļrakstīšanas instalāciju/savienojamību
  - Ir radusies problēma ar Azure AD Connect instalēšanu/savienojamību
  - Papildinformāciju par problēmu novēršanu saistībā ar paroļu arī atpakaļrakstīšanas skatiet rakstā [paroļu arī atpakaļrakstīšanas problēmu novēršana](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Es nezinu, kā atiestatīt lietotāja paroli**

1. Pierakstieties Azure portālā kā atbilstošs administrators.
2. Dodieties uz lapu **lietotāji un grupas** , atlasiet **Visi lietotāji**.
3. Sarakstā atlasiet lietotāju.
4. Atlasītajam lietotājam atlasiet **pārskats** un pēc tam komandjoslā atlasiet **Atiestatīt paroli**.
5. Atlasiet pogu **Atiestatīt paroli** un izpildiet ekrānā redzamos norādījumus.
    - Tiek atiestatīta tikai **Azure portāla** atbalsta paroles arī atpakaļrakstīšanas.

**Atjaunoju lokālā lietotāja paroli no Office 365 administrēšanas portāla vai Office 365 mobilās lietojumprogrammas, taču lietotājs joprojām nevar pierakstīties**

Paroļu arī atpakaļrakstīšanas šajā portālā netiek atbalstīts. Vēlreiz atiestatiet lietotāja paroli Azure portālā.
