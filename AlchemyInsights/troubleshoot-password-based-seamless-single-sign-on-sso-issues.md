---
title: Ar paroli pamatotas vienotās pierakstīšanās (SSO) problēmu novēršana
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9374"
ms.openlocfilehash: 6b4d7335461c913a6b5f782756684c5526a96c58c44853ddf9154aa51607bd4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972831"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Ar paroli pamatotas vienotās pierakstīšanās (SSO) problēmu novēršana

Pamat informāciju par SSO, kuras pamatā ir parole, skatiet rakstā Autentifikācija, kuras pamatā ir [parole, izmantojot Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)

**Ar paroli balstītas SSO konfigurēšana**

1. [Vienotās pierakstīšanās, kuras pamatā ir parole,](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) konfigurēšana — šajā rakstā ir detalizētāku informāciju par opciju, kuras pamatā ir parole. Ja programmai, kuru pievienojat, ir nepieciešama pielāgota konfigurācija un ir jāizmanto paroles SSO, šis raksts ir paredzēts jums.
2. [Vienotās pierakstīšanās, kuras pamatā ir parole, konfigurēšana on-prem programmām](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) — lietojumprogrammas starpniekserveris atbalsta vairākus vienotās pierakstīšanās režīmus. Pierakstīšanās ar paroli ir paredzēta programmām, kas autentifikācijai izmanto lietotājvārda/paroles kombināciju. Kad esat konfigurējis lietojumprogrammai ar paroli balstītu pierakstīsies, lietotājiem būs vienreiz jāpierakstās lokālajā lietojumprogrammā. Pēc tam Azure Active Directory saglabā pierakstīšanās informāciju un automātiski to nodrošina lietojumprogrammai, kad jūsu lietotāji tai piekļūst attāli.
    - Programmai jau vajadzētu būt publicētai un pārbaudītai, izmantojot lietojumprogrammas starpniekserveri. Ja tā nav, izpildiet rakstā Lietojumprogrammu publicēšana, izmantojot [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) lietojumprogrammas starpniekserveri minētās darbības, pēc tam turpiniet ar paroli balstītu SSO konfigurēšanu on-prem lietojumprogrammām.

Lai novērstu ar paroli balstītu SSO, skatiet rakstu Ar paroli pamatotas vienotās [pierakstīšanās pakalpojumā Azure AD problēmu novēršana](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
