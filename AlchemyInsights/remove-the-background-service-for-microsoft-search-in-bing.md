---
title: Microsoft Search fona pakalpojuma noņemšana pakalpojumā Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816203"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a>Microsoft Search fona pakalpojuma noņemšana pakalpojumā Bing

Lai programmā Bing noņemtu Microsoft Search fona pakalpojumu, varat izmēģināt tālāk norādītos līdzekļus.

1. Lai atgrieztos pie sākotnējā meklēšanas dzinēja iestatījumiem, rīkojieties šādi:

    izveide. Pārslēdziet **opciju izmantot Bing kā noklusējuma meklēšanas [](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) programmu**.

    b. [Dodieties uz Microsoft 365 administrēšanas centru](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) un notīriet iestatījumu, kas ietekmē visus lietotājus savā organizācijā.

2. Lai noņemtu fona pakalpojumu no atsevišķas ierīces, veiciet tālāk norādītās darbības.

    izveide. Izvēlieties **vadības paneļa > programmas > programmas un līdzekļi**.

    b. Instalēto programmu sarakstā ar peles labo pogu noklikšķiniet uz **Microsoft meklēšana pakalpojumā Bing** un pēc tam noklikšķiniet uz **Atinstalēt**.

3. Lai noņemtu fona pakalpojumu no vairākām ierīcēm savā organizācijā, piesakieties kā administrators un izpildiet tālāk norādīto komandu skriptā. 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
