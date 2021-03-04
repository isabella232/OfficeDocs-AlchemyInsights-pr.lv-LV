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
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430222"
---
# <a name="troubleshoot-sspr"></a>SSPR problēmu novēršana

**Radās problēmas, konfigurējot paroles atiestatīšanu**

- Ja esat administrators un meklējat, kā iespējot pašapkalpošanās paroles atiestatīšanu, skatiet rakstu [apmācība IESPĒJOT SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), lai konfigurētu paroles atiestatīšanu savai organizācijai. Jūs, iespējams, vēlēsities pārskatīt [licencēšanas prasības](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support). Jūsu organizācijā jābūt piešķirtai vismaz vienai licencei.
    - **Tikai mākoņi** — visi Office 365 (O365) apmaksātie SKU vai Azure AD Basic
    - **Mākoņa un/vai Lokālie lietotāji** — Azure AD Premium P1 vai P2, Enterprise Mobility + Security (EMS) vai Secure ražīgs uzņēmums (SPE)
- Lai saņemtu papildu jautājumus par pašapkalpošanās paroles atiestatīšanu, pārskatiet [mūsu bieži uzdotie jautājumi](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).

**Saņemu kļūdas ziņojumu**

Izlasiet šo rakstu, lai atrastu biežāk sastopamās kļūdas un to risinājumus: problēmu novēršana pašapkalpošanās [paroles atiestatīšanai](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Man radās problēma ar paroles atiestatīšanas politiku**

- Ja paroles atiestatīšanas politika nedarbojas, kā paredzēts, vai jums ir jautājumi par paroļu atiestatīšanas politikām, pārskatiet šo rakstu: [paroļu politikas un ierobežojumi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).
- Paroļu atiestatīšanas politikas neattiecas uz administratoriem. Microsoft ievieš spēcīgu noklusējuma divu vārtu paroles atiestatīšanas politiku jebkurai Azure administratora lomai. Pārliecinieties, vai testējat lietotāju, kurš nav administrators. Papildinformāciju par administratoru atiestatīšanas politiku skatiet šajā rakstā: [administrators atiestatiet politikas atšķirības](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).

**Nevēlos, lai lietotāji reģistrētu papildu drošības informāciju paroles atiestatīšanai**

Jūs varat iepriekš aizpildīt datus (e-pastu un tālruņa atribūtus) saviem lietotājiem, izmantojot API, PowerShell vai Azure AD Connect. Lai uzzinātu, kā lasīt:

- [Paroles atiestatīšanas izvietošana bez nepieciešamības lietotājiem reģistrēties](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Kādus datus izmanto paroles atiestatīšana](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Vēlos, lai lietotāji reģistrētu savu papildu drošības informāciju paroles atiestatīšanai**

1. Lieciet lietotājiem reģistrēt savu drošības informāciju par pašapkalpošanās paroles atiestatīšanu, novirzot tos uz [aka.MS/ssprsetup](https://mysignins.microsoft.com/security-info).
1. Pēc tam, kad dati ir aizpildīti lietotājam (lietotājs vai administrators), virziet lietotāju uz [aka.MS/sspr](https://passwordreset.microsoftonline.com/) , lai jūsu lietotāji varētu būt pilnvaroti atiestatīt savas paroles.
1. Ja lietotāji joprojām saskaras ar problēmām, kas var būt **izplatītākie** vai **paroļu hashi sinhronizētie** lietotāji. Tas nozīmē, ka ir iespējamas problēmas ar paroļu arī atpakaļrakstīšanas pakalpojumu.