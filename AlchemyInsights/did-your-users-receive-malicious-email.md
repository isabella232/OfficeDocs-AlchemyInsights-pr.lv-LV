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
ms.openlocfilehash: 608e2226c055f58ecf4f62e3c913106a6d319190ed6b317508e41514c12ba5d0
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/11/2021
ms.locfileid: "57893410"
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
