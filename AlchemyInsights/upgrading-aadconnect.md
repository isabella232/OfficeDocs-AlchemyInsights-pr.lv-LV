---
title: 932 modernizāciju AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 07de6f8df7bfda2060977c7d5bc6a01766bf3c0a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/28/2019
ms.locfileid: "35365910"
---
# <a name="upgrade-azure-ad-connect"></a>Jaunināšanas debeszils AD savienojumu

Pēc noklusējuma ir iespējota automātiska jaunināšana Azure AD savienojumu, kas palīdz nodrošināt jūs lietojat jaunāko versiju. Lai pārbaudītu automātiskās jaunināšanas iestatījumus, izmantojiet cmdlet **Get ADSyncAutoUpgrade** Azure AD PowerShell. Cmdlet atgriež vienu no šīm vērtībām:

- **Enabled**: automātisks jauninājums ir iespējota.

- **Atspējots**: automātisks jauninājums ir atspējota.

- **Apturēts**: sistēma vairs nav tiesības saņemt automātisku jaunināšanu. Nevar konfigurēt šo vērtību; to iestata sistēma.

Papildinformāciju skatiet sadaļā [Automātiskā jaunināšana](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Lai lejupielādētu jaunāko versiju Azure AD savienojumu, dodieties uz [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).
