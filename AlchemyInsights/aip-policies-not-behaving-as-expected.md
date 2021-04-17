---
title: 'AIP: politikas nedarbojas, kā paredzēts'
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
- "9002266"
- "4780"
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821634"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="a5768-102">AIP: politikas nedarbojas, kā paredzēts</span><span class="sxs-lookup"><span data-stu-id="a5768-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="a5768-103">Azure informācijas aizsardzība: politikas nedarbojas, kā paredzēts, skatiet tālāk sniegtās vadlīnijas dažādām politikas problēmām.</span><span class="sxs-lookup"><span data-stu-id="a5768-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="a5768-104">Ja rodas problēmas ar vizuāliem atzīmēm, lūdzu, [pārskatiet, kad tiek lietoti vizuālie apzīmējumi.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)</span><span class="sxs-lookup"><span data-stu-id="a5768-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="a5768-105">Ja rodas problēmas ar automātisko etiķetēšanu, lūdzu, pārskatiet kā konfigurēt automātiskās un ieteicamās [Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) informācijas aizsardzības klasifikācijas nosacījumus un Ko meklē [sensitīvās informācijas tipi](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="a5768-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="a5768-106">Ja rodas problēmas ar vietējo/Pfile aizsardzību, lūdzu, pārskatiet [failu API konfigurāciju.](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)</span><span class="sxs-lookup"><span data-stu-id="a5768-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="a5768-107">Pārbaudiet, vai izmantojat nepareizi konfigurētas tvēruma politikas: Kā konfigurēt Azure informācijas aizsardzības politiku konkrētiem lietotājiem, [izmantojot tvēruma politikas.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)</span><span class="sxs-lookup"><span data-stu-id="a5768-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="a5768-108">Ja automātiskā marķēšana nedarbojas programmā Outlook, pievienojot marķētu dokumentu, pārliecinieties, vai DRMEncryptProperty nav definēts šeit: [IRM](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)reģistra iestatījumi drošībai .</span><span class="sxs-lookup"><span data-stu-id="a5768-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="a5768-109">Ja joprojām pastāv problēmas, lūdzu, apkopojiet Azure informācijas aizsardzības klienta žurnālus un pievienojiet eksportētos žurnālus šai biļetei.</span><span class="sxs-lookup"><span data-stu-id="a5768-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="a5768-110">Atveriet Office dokumentu vai izveidojiet jaunu e-pasta ziņojumu programmā Outlook.</span><span class="sxs-lookup"><span data-stu-id="a5768-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="a5768-111">Noklikšķiniet **uz Aizsargāt/jūtīgumu**  >  **palīdzība un atsauksmes.**</span><span class="sxs-lookup"><span data-stu-id="a5768-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="a5768-112">Noklikšķiniet **uz Eksportēt žurnālus.**</span><span class="sxs-lookup"><span data-stu-id="a5768-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="a5768-113">Saglabājiet žurnālus savā atrašanās vietā un pievienojiet tos šim pakalpojuma pieprasījumam.</span><span class="sxs-lookup"><span data-stu-id="a5768-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="a5768-114">Papildu resursi:</span><span class="sxs-lookup"><span data-stu-id="a5768-114">Additional resources:</span></span>

- [<span data-ttu-id="a5768-115">Kā konfigurēt etiķeti vizuāliem apzīmējumiem Azure informācijas aizsardzībai</span><span class="sxs-lookup"><span data-stu-id="a5768-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="a5768-116">Azure informācijas aizsardzības dokumentācijas pārskatīšana</span><span class="sxs-lookup"><span data-stu-id="a5768-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="a5768-117">Sensitivitātes etiķešu izmantošana Microsoft 365 programmās</span><span class="sxs-lookup"><span data-stu-id="a5768-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

