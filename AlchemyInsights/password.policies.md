---
title: Paroļu politikas
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 12751288d04a2ec5993bf4a546b7d0c862f8f171f5bfd7a337cb79cb95792056
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040837"
---
# <a name="password-policies"></a>Paroļu politikas

**Radušās problēmas ar lietotāja paroļu politiku**

- Lietotāja paroļu politika ir atkarīga no tā, vai lietotājs ir tikai mākonī vai lokāli.
- Tikai mākonī lietotājiem ir jāizvēlas parole, kas atbilst šajā rakstā prasībām. Paroļu [politikas, kas attiecas tikai uz mākoņa lietotāju kontiem](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)
- Lokālajiem lietotājiem ir jāizvēlas parole, kas atbilst lokālām prasībām. Ja lokāls lietotājs nevar iestatīt savu paroli, pārbaudiet lokālās prasības.

**Es nezinu, kā iestatīt vai pārbaudīt paroļu derīguma politikas**

- Izmantojot PowerShell, varat iestatīt un pārbaudīt mākoņa lietotāju termiņa politiku savā nomniekā. Izpildiet norādījumus šajā rakstā: [Paroļu politiku iestatīšana vai pārbaude, izmantojot PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- Lokālā e-pasta konta lietotāju paroles derīguma termiņa politika ir iestatīta jūsu lokālajā AD.

**Citas noderīgas saites:**
- [Darba sākšana ar paroles atiestatīšanu](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [Administratora iniciēta paroles atiestatīšanas problēmu novēršana](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
