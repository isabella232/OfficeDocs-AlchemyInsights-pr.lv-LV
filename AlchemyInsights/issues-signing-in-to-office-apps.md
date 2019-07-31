---
title: Pierakstīšanās pakalpojumā Office apps jautājumiem
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
- "2560"
ms.openlocfilehash: de0a1b78724db9a8e93d8d599ce3b503abcb86e2
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938269"
---
# <a name="fixing-the-office-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Nosakot Biroja apps "Atvainojiet, citam kontam no uzņēmuma jau pierakstījies" ziņojums

Lai novērstu šo kļūdu, rīkojieties šādi:

- Noņemt visu darbu konti, izņemot skarto kontā, izmantojot Windows iestatījumos > **pieeja darbā vai skolā**.
- [Notīrīt biroja akreditācijas datus](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) , izmantojot Windows Credential Manager.<br/>
    **Piezīme:** Ir mainījušies 16,0 Office 2016 reģistra ceļus. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Atveriet Office app, izvēlieties **failu** > **konta** > **Sign Out**. Pierakstieties, izmantojot lietotāja kontu ar derīgu licenci. Detalizētu informāciju skatiet [Accounts birojā](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Mac, skatiet sadaļā [nevar pierakstīties Office 2016 Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Lai iegūtu papildinformāciju, skatiet ["Atvainojiet, citam kontam no uzņēmuma jau pierakstījies šajā datorā" Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).