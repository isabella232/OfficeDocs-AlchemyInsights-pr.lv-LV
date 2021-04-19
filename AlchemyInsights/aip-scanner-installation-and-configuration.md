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
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="e731e-102">AIP skeneris: instalēšana un konfigurācija</span><span class="sxs-lookup"><span data-stu-id="e731e-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="e731e-103">**Lai instalētu AIP skeneri, izpildiet ieteicamās vadlīnijas:**</span><span class="sxs-lookup"><span data-stu-id="e731e-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="e731e-104">Ja veicat jaunināšanu un neveicat tīru instalāciju, lūdzu, pārliecinieties, vai izpildījāt norādījumus par [Azure informācijas](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) aizsardzības skenera un vienotās uzlīmju klienta jaunināšanas jaunināšanu, skatiet rakstu Azure informācijas aizsardzības [skenera jaunināšana.](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)</span><span class="sxs-lookup"><span data-stu-id="e731e-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="e731e-105">Pārliecinieties, vai ievērojiet [visas ugunsmūru un tīkla infrastruktūras iestatījumu prasības.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)</span><span class="sxs-lookup"><span data-stu-id="e731e-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="e731e-106">Pārliecinieties, [vai jūsu politikām](https://docs.microsoft.com/azure/information-protection/configure-policy) ir iestatīta automātiska marķēšana vai politikā ir noklusējuma etiķete.</span><span class="sxs-lookup"><span data-stu-id="e731e-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="e731e-107">Pārliecinieties, vai atbilstošais faila tips ir konfigurēts uzlīmju/aizsardzības vajadzībām, kā aprakstīts rakstā Failu tipi, [ko atbalsta Azure informācijas aizsardzības klients.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection)</span><span class="sxs-lookup"><span data-stu-id="e731e-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="e731e-108">Turklāt, ja vēlaties mainīt noklusējuma darbību, izpildiet šīs vadlīnijas: [Failu noklusējuma aizsardzības līmeņa maiņa.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)</span><span class="sxs-lookup"><span data-stu-id="e731e-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="e731e-109">Pārbaudiet, vai lietotāja kontam, kas konfigurēts palaist skenera pakalpojumu, ir atļaujas piekļūt visiem konfigurētajiem repozitorijiem.</span><span class="sxs-lookup"><span data-stu-id="e731e-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="e731e-110">Ja problēmas joprojām pastāv, lūdzu, eksportējiet skenera žurnālus un pievienojiet tos atbalsta biļetei.</span><span class="sxs-lookup"><span data-stu-id="e731e-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="e731e-111">**Azure informācijas aizsardzības skenera žurnālu eksportēšana**</span><span class="sxs-lookup"><span data-stu-id="e731e-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="e731e-112">Naviģējiet uz %localappdata%\Microsoft\MSIP zem lietotāja konteksta, kurā darbojas skenera pakalpojums.</span><span class="sxs-lookup"><span data-stu-id="e731e-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="e731e-113">Tilpsaspiesiet visu mapes MSIP saturu.</span><span class="sxs-lookup"><span data-stu-id="e731e-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="e731e-114">Saglabājiet žurnālus paša izvēlētā atrašanās vietā un pievienojiet tos savam pakalpojuma pieprasījumam.</span><span class="sxs-lookup"><span data-stu-id="e731e-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="e731e-115">Varat arī izmantot [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span><span class="sxs-lookup"><span data-stu-id="e731e-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="e731e-116">**Papildinformāciju skatiet rakstā:**</span><span class="sxs-lookup"><span data-stu-id="e731e-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="e731e-117">Azure informācijas aizsardzības skenera izvietošana, lai automātiski klasificētu un aizsargātu failus</span><span class="sxs-lookup"><span data-stu-id="e731e-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="e731e-118">Set-AIPAuthentication parametra Token norādīšana un izmantošana</span><span class="sxs-lookup"><span data-stu-id="e731e-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="e731e-119">Palaidiet atklāšanas ciklu un skatiet skenera atskaites</span><span class="sxs-lookup"><span data-stu-id="e731e-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="e731e-120">Pakalpojuma Azure informācijas aizsardzība dokumentācijas pārskatīšana</span><span class="sxs-lookup"><span data-stu-id="e731e-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="e731e-121">Pakalpojuma Azure informācijas aizsardzība prasības</span><span class="sxs-lookup"><span data-stu-id="e731e-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="e731e-122">Pakalpojuma Azure informācijas aizsardzība klienta lejupielāde</span><span class="sxs-lookup"><span data-stu-id="e731e-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
