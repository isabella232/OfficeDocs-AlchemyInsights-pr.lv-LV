---
title: Tikai lasāmi uzturēšanas ziņojumi, mēģinot izmantot SharePoint vai OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670839"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="234d4-102">Tikai lasāmi uzturēšanas ziņojumi, mēģinot izmantot SharePoint vai OneDrive</span><span class="sxs-lookup"><span data-stu-id="234d4-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="234d4-103">Lietotāji var saņemt **tikai lasāmus uzturēšanas** ziņojumus, mēģinot izmantot SharePoint vai OneDrive vienam no šiem scenārijiem.</span><span class="sxs-lookup"><span data-stu-id="234d4-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="234d4-104">Plānotas vai aktīvas uzturēšanas darbības.</span><span class="sxs-lookup"><span data-stu-id="234d4-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="234d4-105">Pārbaudiet, vai jums ir navigācija uz [ziņojumu centru](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="234d4-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="234d4-106">Augsta prioritāte, aktīvais pakalpojuma incidents, kas var notikt.</span><span class="sxs-lookup"><span data-stu-id="234d4-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="234d4-107">Pārbaudiet, vai nav padomu/incidentu, naviģējot uz [Pakalpojuma darbspējas pakalpojumu](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="234d4-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="234d4-108">Mazs automātiskas atkopšanas scenārijs, kas var rasties, ja rodas neparedzēti notikumi serveros, kas var ilgt mazāk nekā 30 minūtes.</span><span class="sxs-lookup"><span data-stu-id="234d4-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="234d4-109">Šiem nedaudzajiem atklājumiem nav ziņojumu centra vai pakalpojumu darbspējas ziņu, bet jums ir jāatgriežas pavisam drīz.</span><span class="sxs-lookup"><span data-stu-id="234d4-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="234d4-110">Daži gadījumi, kad mēs novērojām, ka viens no trim iepriekš norādītajiem scenārijiem ir cēlonis, un pakalpojums ir atjaunots, bet lietotāju pārlūka kešatmiņa nav notīrīta.</span><span class="sxs-lookup"><span data-stu-id="234d4-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="234d4-111">Lūdzu, mēģiniet notīrīt pārlūkprogrammas kešatmiņu pirms naviģēšanas uz vietni.</span><span class="sxs-lookup"><span data-stu-id="234d4-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="234d4-112">Pārlūkprogrammā Microsoft Edge atlasiet **Iestatījumi**un pēc tam atlasiet **Konfidencialitāte un drošība**.</span><span class="sxs-lookup"><span data-stu-id="234d4-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="234d4-113">Sadaļā **Notīrīt pārlūkošanu**atlasiet **izvēlēties, ko notīrīt**.</span><span class="sxs-lookup"><span data-stu-id="234d4-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="234d4-114">Atlasiet **Sīkfaili un saglabātie tīmekļa vietnes dati**un atlasiet **Notīrīt**.</span><span class="sxs-lookup"><span data-stu-id="234d4-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="234d4-115">Šīs darbības var atšķirties, ja izmantojat citas pārlūkprogrammas, piemēram, Mozilla Firefox vai Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="234d4-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="234d4-116">Vēl viena iespēja ir atvērt SharePoint vietni vai pakalpojumu OneDrive jaunā InPrivate logā.</span><span class="sxs-lookup"><span data-stu-id="234d4-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>