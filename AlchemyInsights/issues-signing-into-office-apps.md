---
title: Problēmas ar pierakstīšanos Microsoft 365 programmās
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: b0789a54f48b2850c1dad8651a8209449c805784bea96799f05e67c4bc43fdb0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986898"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Kļūdas ziņojums Microsoft 365 "Datora uzticamās platformas modulis nedarbojas pareizi"

Lai novērstu šo kļūdu, izmēģiniet tālāk norādīto:

- Instalējiet jaunākos atjauninājumus [lietojumprogrammām Windows](https://support.microsoft.com/help/4027667/windows-10-update) [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [Notīriet Office akreditācijas](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) datus, Windows akreditācijas datu pārvaldnieku.<br/>
    **Piezīme.** 2016. Office gada reģistra ceļi ir mainīti uz 16.0. (Piemēram: \Software\Microsoft\Office\16.0\Common\Identity\)
- Mēģiniet lietotāja [atkopšanas procesu,](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) lai izlabotu uzticamā platformas moduļa (TPM) kļūmes.
- Iestatiet EnableADAL = 0, veicot tālāk norādītās darbības.  
    1. Ar peles labo pogu noklikšķiniet Windows Sākums, izvēlieties **Palaist,** ierakstiet **regedit** un pēc tam izvēlieties **Labi**.
    2. Atlasiet **Jā,** lai atļautu reģistra redaktoram veikt izmaiņas jūsu ierīcē.
    3. Reģistra redaktorā pievienojiet **EnableADAL** DWORD vērtību ar iestatījumu **0** sadaļā HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Papildinformāciju skatiet rakstā Savienojuma problēmas pierakstoties pēc atjaunināšanas uz [Office 2016 būvējumu 16.0.7967 Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).