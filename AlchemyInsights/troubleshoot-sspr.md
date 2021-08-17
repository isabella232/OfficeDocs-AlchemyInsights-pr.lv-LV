---
title: SSPR problēmu novēršana
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 9d8184efdc60befd359059c62ea3eb1a14ad7d2a20dade921d4a71e424f52033
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038965"
---
# <a name="troubleshoot-sspr"></a>SSPR problēmu novēršana

**Radušās problēmas ar paroles atiestatīšanas konfigurēšanu**

- Ja esat administrators un vēlaties meklēt, kā iespējot pašapkalpošanās paroles atiestatīšanu, skatiet rakstu Apmācība [par SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)iespējošanu , lai konfigurētu paroles atiestatīšanu savā organizācijā. Iespējams, vēlēsities arī pārskatīt [licencēšanas prasības.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support) Jūsu organizācijā ir jābūt piešķirtai vismaz vienai licencei.
    - **Tikai mākoņa lietotāji** — Office 365 (O365) maksas SKU vai Azure AD Basic
    - **Mākonis un/vai** lokālie lietotāji — Azure AD Premium P1 vai P2, Enterprise Mobility + Security (EMS) vai Secure Productive Enterprise (SPE)
- Papildu jautājumus par pašapkalpošanās paroles atiestatīšanu skatiet mūsu bieži [uzdoto jautājumu sadaļā.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)

**Saņemu kļūdas ziņojumu**

Skatiet šo rakstu, lai atrastu bieži izplatītas kļūdas un to risinājumus. [Pašapkalpošanās paroles atiestatīšanas problēmu novēršana](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Radušās problēmas ar paroles atiestatīšanas politiku**

- Ja paroļu atiestatīšanas politika neatbilst plānotajam vai jums ir jautājumi par paroļu atiestatīšanas politikām, pārskatiet šo rakstu: Paroļu politikas un ierobežojumi [programmā Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).
- Paroles atiestatīšanas politikas neattiecas uz administratoriem. Microsoft īsteno stipru noklusējuma divvārdu paroles atiestatīšanas politiku jebkurai Azure administratora lomai. Pārliecinieties, vai veicat testēšanu ar lietotāju, kurš nav administrators. Papildinformāciju par administratora atiestatīšanas politiku skatiet šajā rakstā: [Administratora atiestatīšanas politikas atšķirības.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)

**Es nevēlos, lai lietotāji reģistrētu papildu drošības informāciju paroles atiestatīšanai**

Varat iepriekš aizpildīt datus (e-pasta un tālruņa atribūtus) saviem lietotājiem, izmantojot API, PowerShell vai Azure AD Savienošana. Lai uzzinātu, kā to lasīt:

- [Paroles atiestatīšanas izvietošana bez nepieciešamības lietotājiem reģistrēties](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Kādi dati tiek izmantoti, atiestatot paroli](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Es vēlos, lai lietotāji reģistrētu savu papildu drošības informāciju paroles atiestatīšanai**

1. Lai lietotāji reģistrē savu drošības informāciju pašapkalpošanās paroles atiestatīšanai, viņus pāraiciniet uz [aka.ms/ssprsetup.](https://mysignins.microsoft.com/security-info)
1. Kad lietotāja (lietotāja vai administratora) dati ir aizpildīti, lietotāju var pāravot [aka.ms/sspr](https://passwordreset.microsoftonline.com/) lai lietotāji varētu atiestatīt savas paroles.
1. Ja lietotājiem joprojām ir radušās problēmas, visticamāk, ka tie ir **federatīvi vai** paroļu **jaukšanas sinhronizēti** lietotāji. Tas nozīmē, ka pastāv problēma ar paroles rakstīšanas pakalpojumu.