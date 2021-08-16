---
title: Uz noteiktiem Office 365 nosūtīto e-pasta ziņojumu automātiska šifrēšana
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
ms.openlocfilehash: 5a285f36aeb814e3b1d361c8cbffd5a6bef0770d10082d24654c7bbda59ce65b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082193"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Uz noteiktiem Office 365 nosūtīto e-pasta ziņojumu automātiska šifrēšana

1. Administrēšanas [Exchange izvēlieties](https://outlook.office365.com/ecp/)Pasta plūsma un > **kārtulas**. 
2. Noklikšķiniet uz **ikonas Jauns (+)** un pēc tam noklikšķiniet uz **Lietot Office 365 ziņojumu šifrēšana tiesību aizsardzību ziņojumiem.**
3. Lodziņā **Nosaukums** ievadiet kārtulas nosaukumu, piemēram, Šifrēt ziņojumus, *kas nosūtīti contoso.com*.
4. Lodziņā **Lietot šo kārtulu, ja** izvēlieties Adresāta > **domēns ir**. 
5. Ievadiet domēna nosaukumu, piemēram, **contoso.com**.
6. Noklikšķiniet uz **ikonas Pievienot (+)** un pēc tam uz **Labi.**
7. Blakus **laukam Veikt tālāk minētās** darbības noklikšķiniet uz **Atlasīt vienu.** 
8. **RMS veidnes nolaižamajā izvēlnē** atlasiet Šifrēt un **pēc tam** noklikšķiniet uz **Labi**. (Ja neredzat šo opciju, tas nozīmē, ka jūsu plānā nav iekļauta automātiskā šifrēšana. Bet varat to pievienot!)
9. Izvēlieties jebkuru neobligāto atlasi (no izvēles izvēles saraksta, ko var veikt šajā brīdī, daudzas no kurām var atstāt ar noklusējuma vienkāršības iestatījumu).
10. Noklikšķiniet uz **Saglabāt**.

> [!IMPORTANT]
> Šo kārtulu vienmēr var atgriezties un rediģēt vēlāk.

Papildinformāciju par šifrēšanas kārtulu izveidi skatiet rakstā Pasta plūsmas kārtulu [definēšana, lai šifrētu e-pasta ziņojumus Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)