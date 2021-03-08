---
title: Automātiska ar konkrētiem domēniem sūtīto Office 365 e-pasta ziņojumu šifrēšana
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526690"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Automātiska ar konkrētiem domēniem sūtīto Office 365 e-pasta ziņojumu šifrēšana

1. [Exchange administrēšanas centrā](https://outlook.office365.com/ecp/)izvēlieties **pasta plūsmas > kārtulas**. 
2. Noklikšķiniet uz **jaunās (+)** ikonas un pēc tam noklikšķiniet uz **lietot Office 365 ziņojumu šifrēšanu un tiesību aizsardzību uz ziņojumiem**.
3. Lodziņā **nosaukums** ievadiet kārtulas nosaukumu, piemēram, *šifrētu ziņojumus, kas nosūtīti uz contoso.com*.
4. Sadaļā **lietot šo kārtulu, ja** izvēlieties **adresātu > domēns**. 
5. Ievadiet tā domēna nosaukumu, piemēram, **contoso.com**.
6. Noklikšķiniet uz ikonas **Add (+)** un pēc tam noklikšķiniet uz **Labi**.
7. Blakus **veikt tālāk norādītās** darbības noklikšķiniet uz **Atlasīt vienu**. 
8. **RMS veidnes** nolaižamajā izvēlnē atlasiet **Šifrēt** un pēc tam noklikšķiniet uz **Labi**. (Ja neredzat šo opciju, tas nozīmē, ka jūsu plānā nav iekļauta automātiskā šifrēšana. Taču jūs varat to pievienot!)
9. Izvēlieties jebkuru neobligātu atlasi (no neobligāto atlases saraksta, ko varat veikt šajā brīdī, no kuriem daudzus var atstāt ar noklusējuma iestatījumu vienkāršībai).
10. Noklikšķiniet uz **Saglabāt**.

> [!IMPORTANT]
> Vienmēr varat atgriezties un rediģēt šo kārtulu vēlāk.

Papildinformāciju par šifrēšanas kārtulu izveidi skatiet rakstā [pasta plūsmas kārtulu definēšana, lai šifrētu e-pasta ziņojumus pakalpojumā Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)