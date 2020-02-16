---
title: Office lietojumprogrammu labošana jūsu konts ir sliktā stāvoklī ziņojums
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969605"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a>Labošana Office Apps "jūsu konts ir sliktā stāvoklī" kļūda

Lai novērstu šo kļūdu, mēģiniet šīs opcijas attiecīgajā datorā:

- Atveriet Office programmu, atlasiet **failu** > **konta** > **Izrakstīties no visiem kontiem**. Pierakstieties vēlreiz, izmantojot lietotāja kontu ar derīgu licenci. Lai iegūtu detalizētu informāciju, skatiet [Office konti](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Notīrīt Office akreditācijas datus](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) , izmantojot Windows akreditācijas datu pārvaldnieku.<br>
  **Piezīme:** Office 2016 reģistra ceļi ir mainījušies 16,0. Piemēram, \Software\Microsoft\Office\16.0\Common\Identity\
- Attiecīgajā datorā, iestatiet EnableADAL = 0, izmantojot šādas darbības:  
     1. Ar peles labo pogu noklikšķiniet uz pogas Windows un atlasiet **palaist**. Lodziņā **Atvērt** ierakstiet **regedit**un pēc tam atlasiet **Labi**.
     2. Atlasiet **Jā** , kad tiek piedāvāts atļaut reģistra redaktoram veikt izmaiņas ierīcē.
    3. Reģistra redaktorā pievienojiet DWORD vērtību EnableADAL ar iestatījumu 0 sadaļā HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.
- Ja kļūda rodas, veidojot savienojumu ar Office 365, izmantojot Office 2013, [Iespējot mūsdienu autentifikācijas](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) Office klienta.

Lai iegūtu papildinformāciju, skatiet [kā novērst-pārlūka lietojumprogrammas, kas nevar pierakstīties Office 365, Azure vai InTune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

