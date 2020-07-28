---
title: Office programmu automātisko atjauninājumu kontrolēšana
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439335"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="90300-102">Office programmu automātisko atjauninājumu kontrolēšana</span><span class="sxs-lookup"><span data-stu-id="90300-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="90300-103">Pēc noklusējuma Office programmu atjauninājumi tiek lejupielādēti automātiski un izmantoti fonā bez lietotāja iejaukšanās.</span><span class="sxs-lookup"><span data-stu-id="90300-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="90300-104">Taču administratori var kontrolēt, kā atjauninājumi tiek lietoti, izmantojot Office atjaunināšanas iestatījumus.</span><span class="sxs-lookup"><span data-stu-id="90300-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="90300-105">Atjaunināšanas iestatījumi ļauj administratoriem iespējot vai atspējot automātisko atjaunināšanu, rādīt vai paslēpt Office **atjaunināšanas** pogu, iestatīt atjaunināšanas termiņus un veikt citas funkcijas.</span><span class="sxs-lookup"><span data-stu-id="90300-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="90300-106">Detalizētu informāciju skatiet rakstā:</span><span class="sxs-lookup"><span data-stu-id="90300-106">For detailed information, see:</span></span>

- [<span data-ttu-id="90300-107">Office atjaunināšanas iestatījumu konfigurēšana</span><span class="sxs-lookup"><span data-stu-id="90300-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="90300-108">Office automātiskā atjaunināšana nav iespējota</span><span class="sxs-lookup"><span data-stu-id="90300-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="90300-109">Kā definēt, kā Office tiek atjaunināts pēc tam, kad tā ir instalēta</span><span class="sxs-lookup"><span data-stu-id="90300-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="90300-110">Lai pārskatītu klienta datoram lietotos atjauninājumus, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="90300-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="90300-111">Atveriet reģistra redaktoru, dodoties uz **Sākt**  >  **palaist**  >  **regedit**.</span><span class="sxs-lookup"><span data-stu-id="90300-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="90300-112">Pārslēdzieties uz šo atrašanās vietu un pārskatiet Office atjaunināšanas iestatījumus.</span><span class="sxs-lookup"><span data-stu-id="90300-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="90300-113">izveide.</span><span class="sxs-lookup"><span data-stu-id="90300-113">a.</span></span> <span data-ttu-id="90300-114">HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft\Office</span><span class="sxs-lookup"><span data-stu-id="90300-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="90300-115">b.</span><span class="sxs-lookup"><span data-stu-id="90300-115">b.</span></span> <span data-ttu-id="90300-116">ClickToRun\Configuration</span><span class="sxs-lookup"><span data-stu-id="90300-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="90300-117">**Piezīmes**  Ja OfficeMgmtCOM atslēga ir iestatīta, iespējams, tiek rādīts ziņojums "atjauninājumi tiek pārvaldīti sistēmas administrators" **Office**  >  **konta**  >  **Office atjauninājumos**.</span><span class="sxs-lookup"><span data-stu-id="90300-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="90300-118">Papildinformāciju skatiet rakstā [microsoft 365 programmu atjauninājumu pārvaldība, izmantojot Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="90300-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  