---
title: Vai jūsu lietotāji saņēmuši ļaunprātīgu e-pasta ziņojumu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: de8823253d60efcd38bfa96864c146a2cedc0537f6d0aa41de6dafc6c7debc03
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929204"
---
# <a name="did-your-users-receive-malicious-email"></a>Vai jūsu lietotāji saņēmuši ļaunprātīgu e-pasta ziņojumu?

- Tagad varat ziņot par ļaunprātīgu e-pastu korporācijai Microsoft, izmantojot [Administrēšanas iesniegumus Drošības un atbilstības centrā](https://sip.protection.office.com/reportsubmission).

Ziņojumi, kas tiek iesniegti [administratora iesniegumos](https://sip.protection.office.com/reportsubmission), tiek skenēti, un šādi rezultāti tiks parādīti **detalizētajā informatīvajā** lapā:

- Ja piegādes laikā sūtītāja e-pasta autentifikācijā bija kļūme.
- Informācija par visiem politikas trāpījumiem, kas varētu būt ietekmējuši vai ignorējuši ziņojuma spriedumu.
- Pašreizējie detonācijas rezultāti, lai noskaidrotu, vai ziņojumā ietvertie vietrāži URL vai faili ir vai nav ļaunprātīgi.
- Atsauksmes no vērtētājiem

Ja tika konstatēts ignorēšana, atkārtotai skenēšanai vajadzētu būt pabeigtai pēc dažām minūtēm. Ja nebija problēmas ar e-pasta autentifikāciju vai piegādi neietekmēja ignorēšana, vērtētāju atsauksmes var ilgt pat vienu dienu.

Ja nepiekrītat galējam verdiktam, vietrāža URL vai failam (bloķēts vai nav bloķēts), pēc dienas atkal iesniedziet ziņojumu atkārtotai nosūtīšanai. Ir ļoti iespējams, ka verdikts mainīsies pēc atkārtotas ziņojuma iesniegšanas.

Tikmēr varat noņemt ļaunprātīgu e-pastu no lietotāju iesūtnēs, izpildot norādījumus, kas sniegti [šajā rakstā](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- Klienti, kuri lieto Microsoft Defender pakalpojumam Office 365, var:
    - Izmantojiet [Draudu pārlūks, lai atrastu un izdzēstu aizdomīgu e-pastu](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
    - [izmantojiet drošās saites, lai bloķētu piekļuvi](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) ļaunprātīgam vietrādim URL
    - izsekojiet lietotājiem, kuri noklikšķinājis un piekļuvis ļaunprātīgiem vietrāžiem URL: [Skatiet pikšķerēšanas vietrāža URL un noklikšķiniet uz verdikta datiem](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
    - manuāli [sākt automatizēta izmeklēšana](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Varat arī aizsargāt pret ļaunprātīgiem failiem un vietrāžiem URL, izpildot norādījumus, kas sniegti sadaļā [Aizsardzība pret ļaunprātīgiem vietrāžiem URL un failiem](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).