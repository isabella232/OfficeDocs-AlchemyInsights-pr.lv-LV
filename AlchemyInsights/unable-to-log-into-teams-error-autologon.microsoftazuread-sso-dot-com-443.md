---
title: Nevar pieteikties programmā Teams, jo radās kļūda autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 6671a63d97f24fadc9b34907d75600a3c0ad1c9990a4a8f8d32034c11e8a952e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038407"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>Nevar pieteikties programmā Teams, jo radās kļūda autologon.microsoftazuread-sso dot com:443

Ja Seamless SSO ir iespējots kā O365 autentifikācija, iespējams, ka iekštīkla vietnēm ir jāpievieno URL “autologon.microsoftazuread-sso.com”.  Ja tas iepriekš ir bijis pievienots uzticamajām vietnēm un tiek lietots Seamless SSO, tas no uzticamajām vietnēm ir jānoņem.

Lūdzu, izskatiet [Seamless SSO problēmu novēršanas kontrolsarakstu](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).

Veiciet tālāk norādītās darbības, lai pievienotu URL iekštīkla vietņu sarakstam.

1. Atveriet pārlūkprogrammu Internet Explorer, noklikšķinot uz pogas **Sākt**. Meklēšanas lodziņā ierakstiet Internet Explorer un pēc tam rezultātu sarakstā noklikšķiniet uz **Internet Explorer**.
2. Noklikšķiniet uz **Rīki** un pēc tam noklikšķiniet uz **Interneta opcijas**.
3. Noklikšķiniet uz cilnes **Drošība**.
4. Tagad noklikšķiniet uz **Lokālā iekštīkla vietnes** un pēc tam noklikšķiniet uz pogas **Vietnes**, un pēc tam uz pogas **Papildu**.
5. Ievadiet tīmekļa vietnes URL un noklikšķiniet uz **Pievienot**.
6. Kad tas ir izdarīts, noklikšķiniet uz **Saglabāt**.

Papildinformāciju skatiet rakstā [Dokumentācija Seamless SSO izvietošanai pakalpojumā O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (3. darbībā ietverts uz politikas balstīts process URL pievienošanai iekštīkla vietnēs).
