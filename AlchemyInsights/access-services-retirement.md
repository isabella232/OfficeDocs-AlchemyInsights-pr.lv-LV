---
title: Piekļuves pakalpojumu pensionēšanās
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 197366882468ebc87fc26f2fe2733371790d1871
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/18/2019
ms.locfileid: "36747791"
---
# <a name="access-services-retirement"></a><span data-ttu-id="7e8de-102">Piekļuves pakalpojumu pensionēšanās</span><span class="sxs-lookup"><span data-stu-id="7e8de-102">Access services retirement</span></span>

<span data-ttu-id="7e8de-103">Kā mēs sākotnēji paziņoja MC97576, martā 2017, un turpināja sazināties pēdējo gadu piekļuves pakalpojumi tiek pārtraukts no Office 365.</span><span class="sxs-lookup"><span data-stu-id="7e8de-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="7e8de-104">Nākamā fāze šajā procesā būs Access Web datu bāzu noņemšana, kas izmanto SharePoint sarakstus kā pamatā esošo datu krātuvi.</span><span class="sxs-lookup"><span data-stu-id="7e8de-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="7e8de-105">**Kā tas ietekmē mani?**</span><span class="sxs-lookup"><span data-stu-id="7e8de-105">**How does this affect me?**</span></span>

<span data-ttu-id="7e8de-106">Sākot Jūnijs 2019, mēs pārtraukt jaunu Access datu bāzes izveide SharePoint Online un izslēdziet pakalpojumu un visas pārējās programmas gada 2020.</span><span class="sxs-lookup"><span data-stu-id="7e8de-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="7e8de-107">**Kas man jādara, lai sagatavotos šīm izmaiņām?**</span><span class="sxs-lookup"><span data-stu-id="7e8de-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="7e8de-108">Mēs aicinām jūs izveidot pārejas plānu jūsu organizācijas Access Web datu bāzēm.</span><span class="sxs-lookup"><span data-stu-id="7e8de-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="7e8de-109">Administratori var izmantot [SharePoint Access lietojumprogrammas skeneri](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) , lai iegūtu to piekļuves programmu sarakstu, kuras izmanto vietnes.</span><span class="sxs-lookup"><span data-stu-id="7e8de-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="7e8de-110">Ir vairāki veidi, kā migrēt Access Web datu bāzes datus:</span><span class="sxs-lookup"><span data-stu-id="7e8de-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="7e8de-111">Importēšana lokālā Access datu bāzē (. ACCDB) vai Excel failā.</span><span class="sxs-lookup"><span data-stu-id="7e8de-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="7e8de-112">Ieteicams arī izpētīt Microsoft PowerApps kā alternatīvu platformu, lai izveidotu bez koda biznesa risinājumus Web un mobilajām ierīcēm.</span><span class="sxs-lookup"><span data-stu-id="7e8de-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>