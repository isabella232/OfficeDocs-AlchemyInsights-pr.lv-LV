---
title: 'AIP skeneris: uzstādīšana un konfigurēšana'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: d059d411aef03ca57662b71fbd7d27aecd3e0e57
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358100"
---
# <a name="aip-scanner-installation-and-configuration"></a>AIP skeneris: uzstādīšana un konfigurēšana

**Lai uzstādītu AIP skeneri, izpildiet ieteiktās vadlīnijas**.

1. Ja veicat jaunināšanu un neveicat tīro instalēšanu, pārliecinieties, vai esat izpildījis norādījumus par [Azure informācijas aizsardzības skenera](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) un vienotā marķēšanas klienta jaunināšanu, skatiet sadaļu [Azure informācijas aizsardzības skenera jaunināšana](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).
2. Pārbaudiet, vai ievērojat visus [ugunsmūrus un tīkla infrastruktūras iestatījumu prasības](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).
3. Pārliecinieties, vai jūsu [politikām ir iestatīta](https://docs.microsoft.com/azure/information-protection/configure-policy) automātiskā marķēšana vai noklusējuma etiķete politikā.
4. Pārliecinieties, vai attiecīgais faila tips ir konfigurēts etiķetei/aizsardzībai, kā aprakstīts [Azure informācijas aizsardzības klienta atbalstītajos failu tipos](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection). Turklāt, ja vēlaties mainīt noklusējuma uzvedību, izpildiet šīs vadlīnijas: [failu noklusējuma aizsardzības līmeņa maiņa](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. Pārbaudiet, vai lietotāja konts konfigurēts, lai palaistu skenera pakalpojums ir atļaujas piekļūt konfigurēto krātuvēs.
6. Ja joprojām rodas problēmas, lūdzu, eksportējiet skenera žurnālus un pievienojiet tos atbalsta biļetei.

**Azure informācijas aizsardzības pārbaudes rīka žurnālu eksportēšana**

1. Naviģējiet uz% LOCALAPPDATA%\microsoft\msip saskaņā ar lietotāja kontekstu, kurā darbojas skenera pakalpojums.
2. Zip visu saturu ar MSIP mapi.
3. Saglabājiet žurnālus savā izvēlētā atrašanās vietā un pievienojiet tos pakalpojuma pieprasījumam.
4. Jūs varat arī izmantot [Export-AIPLogs-OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**Lai iegūtu papildu informāciju, skatiet**:
- [Azure informācijas aizsardzības skenera izvietošana, lai automātiski klasificētu un aizsargātu failus](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Norādiet un izmantojiet marķiera parametru Set-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Atklāšanas cikla palaišana un skenera atskaišu skatīšana](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Azure informācijas aizsardzības dokumentācijas pārskatīšana](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Prasības Azure informācijas aizsardzība](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Lejupielādēt Azure informācijas aizsardzības klients](https://www.microsoft.com/download/details.aspx?id=53018)
