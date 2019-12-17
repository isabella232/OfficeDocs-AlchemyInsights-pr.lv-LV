---
title: Tikai lasāms uzturēšanas ziņojums, mēģinot izmantot SharePoint vai OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051288"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="6a729-102">Tikai lasāms uzturēšanas ziņojums, mēģinot izmantot SharePoint vai OneDrive</span><span class="sxs-lookup"><span data-stu-id="6a729-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="6a729-103">Lietotāji var saņemt **tikai lasāms uzturēšanas** ziņojumu, mēģinot izmantot SharePoint vai OneDrive vienam no šiem scenārijiem.</span><span class="sxs-lookup"><span data-stu-id="6a729-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="6a729-104">Plānotā vai aktīvā uzturēšanas aktivitāte.</span><span class="sxs-lookup"><span data-stu-id="6a729-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="6a729-105">Pārbaudiet tās, pārejot uz [ziņu centru](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="6a729-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="6a729-106">Kas var būt ļoti prioritārs un aktīvs pakalpojumu gadījums.</span><span class="sxs-lookup"><span data-stu-id="6a729-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="6a729-107">Pārbaudiet, vai nav konsultācijas/incidentu, pārejot uz [pakalpojumu veselību](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="6a729-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="6a729-108">Nelielas automātiskās sadzīšana atgūšana scenārijs, kas varētu notikt sakarā ar jebkuru negaidītu notikumu serveros, kas varētu ilgt mazāk nekā 30 min, vai arī tā.</span><span class="sxs-lookup"><span data-stu-id="6a729-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="6a729-109">Nav ziņu centru vai pakalpojumu veselības amati šīs nelielas atgūšanas, bet jums vajadzētu būt atpakaļ normālā ļoti drīz.</span><span class="sxs-lookup"><span data-stu-id="6a729-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="6a729-110">Ļoti retos gadījumos mēs novērots, ka viens no trim scenārijiem uzskaitīti iepriekš ir iemesls, un pakalpojums ir atjaunota, bet lietotājiem pārlūka kešatmiņu nav noskaidroti augšu.</span><span class="sxs-lookup"><span data-stu-id="6a729-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="6a729-111">Lūdzu, mēģiniet notīrīt pārlūka kešatmiņu pirms navigāciju uz vietni.</span><span class="sxs-lookup"><span data-stu-id="6a729-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="6a729-112">Pārlūkprogrammā Microsoft Edge atlasiet **Iestatījumi**un pēc tam atlasiet **Konfidencialitāte un drošība**.</span><span class="sxs-lookup"><span data-stu-id="6a729-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="6a729-113">Sadaļā **Notīrīt pārlūkošanu**atlasiet **izvēlēties, ko notīrīt**.</span><span class="sxs-lookup"><span data-stu-id="6a729-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="6a729-114">Atlasiet **Sīkfaili un saglabātie tīmekļa vietņu dati**un atlasiet **Notīrīt**.</span><span class="sxs-lookup"><span data-stu-id="6a729-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="6a729-115">Šīs darbības var atšķirties, izmantojot citas pārlūkprogrammas, piemēram, Mozilla Firefox vai Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="6a729-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="6a729-116">Cita opcija ir atvērt SharePoint vietni vai OneDrive jaunā InPrivate logā.</span><span class="sxs-lookup"><span data-stu-id="6a729-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>