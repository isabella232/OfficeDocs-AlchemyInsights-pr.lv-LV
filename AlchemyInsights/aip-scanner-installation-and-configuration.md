---
title: 'AIP skeneris: instalēšana un konfigurācija'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: c32f3f10e2e17cf67e73ec8404be293eeefb68a3
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821670"
---
# <a name="aip-scanner-installation-and-configuration"></a>AIP skeneris: instalēšana un konfigurācija

**Lai instalētu AIP skeneri, izpildiet ieteicamās vadlīnijas:**

1. Ja veicat jaunināšanu un neveicat tīru instalāciju, lūdzu, pārliecinieties, vai izpildījāt norādījumus par [Azure informācijas](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) aizsardzības skenera un vienotās uzlīmju klienta jaunināšanas jaunināšanu, skatiet rakstu Azure informācijas aizsardzības [skenera jaunināšana.](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)
2. Pārliecinieties, vai ievērojiet [visas ugunsmūru un tīkla infrastruktūras iestatījumu prasības.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)
3. Pārliecinieties, [vai jūsu politikām](https://docs.microsoft.com/azure/information-protection/configure-policy) ir iestatīta automātiska marķēšana vai politikā ir noklusējuma etiķete.
4. Pārliecinieties, vai atbilstošais faila tips ir konfigurēts uzlīmju/aizsardzības vajadzībām, kā aprakstīts rakstā Failu tipi, [ko atbalsta Azure informācijas aizsardzības klients.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection) Turklāt, ja vēlaties mainīt noklusējuma darbību, izpildiet šīs vadlīnijas: [Failu noklusējuma aizsardzības līmeņa maiņa.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)
5. Pārbaudiet, vai lietotāja kontam, kas konfigurēts palaist skenera pakalpojumu, ir atļaujas piekļūt visiem konfigurētajiem repozitorijiem.
6. Ja problēmas joprojām pastāv, lūdzu, eksportējiet skenera žurnālus un pievienojiet tos atbalsta biļetei.

**Azure informācijas aizsardzības skenera žurnālu eksportēšana**

1. Naviģējiet uz %localappdata%\Microsoft\MSIP zem lietotāja konteksta, kurā darbojas skenera pakalpojums.
2. Tilpsaspiesiet visu mapes MSIP saturu.
3. Saglabājiet žurnālus paša izvēlētā atrašanās vietā un pievienojiet tos savam pakalpojuma pieprasījumam.
4. Varat arī izmantot [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**Papildinformāciju skatiet rakstā:**
- [Azure informācijas aizsardzības skenera izvietošana, lai automātiski klasificētu un aizsargātu failus](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Set-AIPAuthentication parametra Token norādīšana un izmantošana](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Palaidiet atklāšanas ciklu un skatiet skenera atskaites](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Pakalpojuma Azure informācijas aizsardzība dokumentācijas pārskatīšana](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Pakalpojuma Azure informācijas aizsardzība prasības](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Pakalpojuma Azure informācijas aizsardzība klienta lejupielāde](https://www.microsoft.com/download/details.aspx?id=53018)
