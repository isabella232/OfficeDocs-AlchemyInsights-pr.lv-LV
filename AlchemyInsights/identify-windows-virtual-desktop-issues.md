---
title: Windows virtuālās darbvirsmas problēmu identificēšana
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595852"
---
# <a name="identify-windows-virtual-desktop-issues"></a>Windows virtuālās darbvirsmas problēmu identificēšana

Windows virtuālās darbvirsmas diagnostika izmanto tikai vienu PowerShell cmdlet, bet tajā ir daudz neobligātu parametru, lai sašaurinātu un izolētu problēmas. Lai sāktu darbu: 

1. Lejupielādējiet un importējiet Windows virtuālās darbvirsmas PowerShell moduli. Detalizētu informāciju skatiet rakstā [Windows virtuālās darbvirsmas cmdlet čaulai Windows PowerShell.](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)

1. Lai pierakstītos savā kontā, palaidiet šādu cmdlet:
    
    Piemērs: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`

**PIEZĪME.** Visos vaicājumos, izmantojot PowerShell, ir jāiekļauj parametri -UserName vai -ActivityID. Informāciju par pārraudzības iespējām skatiet rakstā [Žurnālu analīzes izmantošana diagnostikas līdzeklim.](https://go.microsoft.com/fwlink/?linkid=2126847)

Lai filtrētu diagnostikas darbības pēc lietotāja, palaidiet šādu cmdlet:

Piemērs: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`

Ir pieejams saraksts ar filtriem, kurus varat palaist, lai diagnosticētu problēmas. Papildinformāciju par problēmu diagnosticēšanu skatiet rakstā [Windows virtuālās darbvirsmas problēmu identificēšana un diagnosticēšana.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)

Papildinformāciju par biežāk sastopamajām kļūdām skatiet [rakstā Bieži sastopamās kļūdas](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).
