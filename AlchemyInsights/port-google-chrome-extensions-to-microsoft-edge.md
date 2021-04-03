---
title: Google Chrome paplašinājumu ports līdz Microsoft Edge (Chromium)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004032"
- "7102"
- "8297"
- "9004617"
ms.openlocfilehash: 1c71d74d01c1e38e4c7789aea2c0b43701b3a5de
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505291"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a>Google Chrome paplašinājumu ports līdz Microsoft Edge (Chromium)

Ir vienkārši pārnesiet [Google Chrome paplašinājumus uz pārlūkprogrammu Microsoft Edge (Chromium).](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension) Lielākajā daļā gadījumu ir nepieciešamas tikai minimālas izmaiņas, lai palaistu šos paplašinājumus programmā Microsoft Edge.

Google Chrome atbalstītie paplašinājuma API un manifesta atslēgas ir ar Microsoft Edge saderīgas ar kodu. Tomēr Microsoft Edge neatbalsta paplašinājuma APIs chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken un chrome.instanceID.