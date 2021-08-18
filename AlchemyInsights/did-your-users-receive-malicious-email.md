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
ms.openlocfilehash: 525af0b29ffa291ddf69f6f2d97f505e93342989
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326682"
---
# <a name="did-your-users-receive-malicious-email"></a>Vai jūsu lietotāji saņēmuši ļaunprātīgu e-pasta ziņojumu?

Tagad varat ziņot par ļaunprātīgu e-pastu korporācijai [Microsoft, izmantojot iesniegšanas Microsoft 365 Defender portālā](https://sip.security.microsoft.com/reportsubmission?viewid=admin).

Ziņojumi, kas tiek iesniegti [administrēšanas iesniegumos,](https://security.microsoft.com/reportsubmission?viewid=admin) tiek skenēti un detalizēti izlidošanas rezultātos redzami šādi rezultāti:

- Ja piegādes laikā sūtītāja e-pasta autentifikācijā bija kļūme.
- Informācija par visiem politikas trāpījumiem, kas varētu būt ietekmējuši vai ignorējuši ziņojuma spriedumu.
- Pašreizējie detonācijas rezultāti, lai noskaidrotu, vai ziņojumā ietvertie vietrāži URL vai faili ir vai nav ļaunprātīgi.
- Atsauksmes no vērtētājiem

Ja tika konstatēts ignorēšana, atkārtotai skenēšanai vajadzētu būt pabeigtai pēc dažām minūtēm. Ja nebija problēmas ar e-pasta autentifikāciju vai piegādi neietekmēja ignorēšana, vērtētāju atsauksmes var ilgt pat vienu dienu.

Ja nepiekrītat galējam verdiktam, vietrāža URL vai failam (bloķēts vai nav bloķēts), pēc dienas atkal iesniedziet ziņojumu atkārtotai nosūtīšanai. Ir ļoti iespējams, ka verdikts mainīsies pēc atkārtotas ziņojuma iesniegšanas.

Tikmēr varat noņemt ļaunprātīgu e-pastu no lietotāju iesūtnēs, izpildot norādījumus, kas sniegti [šajā rakstā](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- Klienti, kuri lieto Microsoft Defender pakalpojumam Office 365, var:
  - Apdraudējumu [pārlūka izmantošana aizdomīga e-pasta atrašanai un dzēšanai](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
  - [Saišu izmantošana Seifs lai bloķētu piekļuvi](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-links) ļaunprātīgam URL
  - Kā izsekot lietotājus, kuri noklikšķināja un piekļuvās ļaunprātīgiem vietrāžiem URL: Skatīt [pikšķerēšanas vietrādi URL](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer)un noklikšķināt uz depozīti dati  &  [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
  - Automātiskas [izmeklēšanas manuāla sākšana](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Varat arī aizsargāt pret ļaunprātīgiem failiem un vietrāžiem URL, izpildot norādījumus, kas sniegti sadaļā [Aizsardzība pret ļaunprātīgiem vietrāžiem URL un failiem](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).
