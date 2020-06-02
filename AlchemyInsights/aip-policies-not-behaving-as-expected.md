---
title: 'AIP: politikas nav uzvedas kā gaidīts'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 7926ff9ebbd54969fb5b3ae5d909baffe96a4292
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/26/2020
ms.locfileid: "44493160"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="2d382-102">AIP: politikas nav uzvedas kā gaidīts</span><span class="sxs-lookup"><span data-stu-id="2d382-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="2d382-103">Azure informācijas aizsardzība: politikas nav uzvedas kā paredzēts, skatiet šo ieteicamās vadlīnijas dažādiem politikas jautājumiem:</span><span class="sxs-lookup"><span data-stu-id="2d382-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="2d382-104">Ja jums ir problēmas ar vizuālām atzīmēm, lūdzu, pārskatiet, [kad tiek lietoti vizuālie marķējumi](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="2d382-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="2d382-105">Ja rodas problēmas ar automātisku marķēšanu, lūdzu, pārskatiet, [kā konfigurēt nosacījumus automātiskai un ieteicamajai klasifikācijai Azure informācijas aizsardzībai](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) un [kāda veida sensitīvo informācijas tipu meklē](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="2d382-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>
3. <span data-ttu-id="2d382-106">Ja rodas problēmas ar vietējo/Pfile aizsardzību, lūdzu, pārskatiet [failu API konfigurāciju](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="2d382-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="2d382-107">Pārbaudiet, ja izmantojat ietverti politikas, kas nav konfigurēti pareizi: [kā konfigurēt Azure informācijas aizsardzības politika noteiktiem lietotājiem, izmantojot ietverti politikas](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="2d382-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="2d382-108">Ja automātiskā marķēšana nedarbojas Outlook, pievienojot dokumentu ar apzīmējumu, pārbaudiet, vai DRMEncryptProperty nav definēts kā aprakstīts šeit: [IRM reģistra iestatījumus drošībai](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="2d382-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="2d382-109">Ja jums joprojām ir radušās problēmas, lūdzu, apkopojiet Azure informācijas aizsardzības klienta žurnālus un pievienojiet eksportētos žurnālus šai biļetei.</span><span class="sxs-lookup"><span data-stu-id="2d382-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="2d382-110">Atveriet Office dokumentu vai izveidojiet jaunu e-pastu programmā Outlook.</span><span class="sxs-lookup"><span data-stu-id="2d382-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="2d382-111">Noklikšķiniet uz **aizsargāt/jutīguma**  >  **Palīdzība un atsauksmes**.</span><span class="sxs-lookup"><span data-stu-id="2d382-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="2d382-112">Noklikšķiniet uz **Eksportēt žurnālus**.</span><span class="sxs-lookup"><span data-stu-id="2d382-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="2d382-113">Saglabājiet žurnālus savā izvēlētā atrašanās vietā un pievienojiet tos šim pakalpojuma pieprasījumam.</span><span class="sxs-lookup"><span data-stu-id="2d382-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="2d382-114">Papildu resursi:</span><span class="sxs-lookup"><span data-stu-id="2d382-114">Additional resources:</span></span>

- [<span data-ttu-id="2d382-115">Kā konfigurēt Visual marķējums etiķete Azure informācijas aizsardzība</span><span class="sxs-lookup"><span data-stu-id="2d382-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="2d382-116">Azure informācijas aizsardzības dokumentācijas pārskatīšana</span><span class="sxs-lookup"><span data-stu-id="2d382-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="2d382-117">Jutības iezīmju izmantošana Office lietojumprogrammās</span><span class="sxs-lookup"><span data-stu-id="2d382-117">Use sensitivity labels in Office apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

