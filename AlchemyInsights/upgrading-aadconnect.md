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
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 210f230929db72027a0f729b17901fe88eb45709
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757298"
---
# <a name="upgrade-azure-ad-connect"></a>Jaunināšanas debeszils AD savienojumu

Pēc noklusējuma ir iespējota automātiska jaunināšana Azure AD savienojumu, kas palīdz nodrošināt jūs lietojat jaunāko versiju. Lai pārbaudītu automātiskās jaunināšanas iestatījumus, izmantojiet cmdlet **Get ADSyncAutoUpgrade** Azure AD PowerShell. Cmdlet atgriež vienu no šīm vērtībām: 

- **Enabled**: automātisks jauninājums ir iespējota.

- **Atspējots**: automātisks jauninājums ir atspējota.

- **Apturēts**: sistēma vairs nav tiesības saņemt automātisku jaunināšanu. Nevar konfigurēt šo vērtību; to iestata sistēma. 

Papildinformāciju skatiet sadaļā [Automātiskā jaunināšana](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Lai lejupielādētu jaunāko versiju Azure AD savienojumu, dodieties uz [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).
