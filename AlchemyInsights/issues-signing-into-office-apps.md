---
title: Problēmas pierakstoties Microsoft 365 Apps
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579872"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Nosakot Microsoft 365 Apps "jūsu datora uzticams platformas modulis nedarbojas pareizi" ziņojums

Lai novērstu šo kļūdu, izmēģiniet tālāk norādīto:

- Instalējiet jaunākos [Windows](https://support.microsoft.com/help/4027667/windows-10-update) un [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)atjauninājumus.
- [Notīrīt Office akreditācijas datus](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) , izmantojot Windows akreditācijas datu pārvaldnieku.<br/>
    **Piezīme:** Office 2016 reģistra ceļi ir mainījušies 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Mēģiniet veikt [lietotāja atkopšanas procesu](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) , lai labotu uzticamā platformas moduļa (TPM) kļūmes.
- Iestatiet EnableADAL = 0, izmantojot šādas darbības:  
    1. Ar peles labo pogu noklikšķiniet uz Windows pogas Sākt, izvēlieties **palaist**, ierakstiet **regedit**, un pēc tam izvēlieties **Labi**.
    2. Atlasiet **Jā** , lai atļautu reģistra redaktoru veikt izmaiņas ierīcē.
    3. Reģistra redaktorā pievienojiet DWORD vērtību **Enableadal** ar iestatījumu **0** sadaļā HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.

Lai iegūtu papildinformāciju, skatiet [savienojuma problēmas pierakstīšanās pēc atjauninājuma Office 2016 veidot 16.0.7967 operētājsistēmā Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).