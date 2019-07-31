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
- "2556"
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938271"
---
# <a name="blank-sign-in-screen-in-office-apps"></a>Tukša pierakstīšanās ekrāna Office programmās

Lai atrisinātu šo problēmu, mēģiniet veikt šādas darbības:
- [Windows](https://support.microsoft.com/help/4027667/windows-10-update) un [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)instalētu jaunākos atjauninājumus.
- Atiestatīt programmas Internet Explorer opcijām: iet uz **Tools** > **Interneta opcijas** > **Advanced** > **Atiestatīt Internet Explorer iestatījumus** (ņemiet vērā, ka jūs zaudēsiet pielāgotos iestatījumus) un pēc tam mēģiniet pierakstīties vēlreiz uz biroju.
- Atspējot Windows Defender programma aizsargs (WDAG) vai līdzīgu firewall vai anti-virus programmu:
    1. Vadības panelī dodieties uz **programmas**un pēc tam izvēlieties **ieslēgt Windows līdzekļu ieslēgšana vai izslēgšana**.
    2. Aktivizējot Windows Defender programma apsardzes, atspējojiet to.<br/>
    **Piezīme:** Jums var būt nepieciešams restartēt datoru.
- Nodrošina, ka Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) nav bloķēti ar jebkuru pieteikumu vai ugunsmūra/anti-virus programmu.
- [Notīrīt biroja akreditācijas datus](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) , izmantojot Windows Credential Manager.<br/>
    **Piezīme:** Ir mainījušies 16,0 Office 2016 reģistra ceļus. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Papildinformāciju skatiet sadaļā [savienojuma problēmas pierakstīšanās pēc Biroja 2016 būvēt 16.0.7967 10 Windows atjauninājums](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).