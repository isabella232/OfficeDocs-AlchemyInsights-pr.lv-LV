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
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714892"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Ar paroli pamatotas vienotās pierakstīšanās (SSO) problēmu novēršana

Lai apgūtu SSO ar paroli pamatotos pamatprincipus, skatiet rakstu [ar paroli pamatota autentifikācija ar Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).

**Ar paroli pamatota SSO konfigurēšana**

1. Ar [paroli pamatotas vienotās pierakstīšanās konfigurēšana](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) . Šajā rakstā ir sniegta detalizēta informācija par SSO opciju ar paroli. Ja pievienojamajai lietojumprogrammai nepieciešama pielāgota konfigurācija un jums ir jāizmanto ar paroli pamatots SSO, šis raksts ir paredzēts jums.
2. Ar [paroli pamatotas vienotās pierakstīšanās konfigurēšana lietojumprogrammā Prem lietojumprogrammas](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) starpniekserveris atbalsta vairākus vienotās pierakstīšanās režīmus. Pierakstīšanās ar paroli ir paredzēts lietojumprogrammām, kas izmanto lietotājvārdu/paroļu kombināciju autentifikācijai. Ja savā lietojumprogrammā konfigurējat pierakstīšanos ar paroli, lietotājiem ir vienreiz jāpierakstās lokālajā lietojumprogrammā. Pēc tam Azure Active Directory saglabā pierakstīšanās informāciju un automātiski nodrošina to lietojumprogrammai, kad lietotāji tam piekļūst attāli.
    - Jūs jau esat publicējis un testējis savu programmu ar lietojumprogrammas starpniekserveri. Ja tā nav, izpildiet darbības, kas aprakstītas sadaļā [lietojumprogrammu publicēšana, izmantojot AZURE ad Application starpniekserveri](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) , un pēc tam turpiniet ar paroli balstītas SSO for on-Prem lietojumprogrammas.

Lai novērstu ar paroli balstītu SSO, skatiet rakstu [ar paroli pamatotas vienotās pierakstīšanās problēmu novēršana AZURE ad](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
