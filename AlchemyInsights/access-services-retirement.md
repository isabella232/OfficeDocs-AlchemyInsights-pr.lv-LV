---
title: Piekļuves pakalpojumu pensijas
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: f5a1e88e4443fdf43cdd4f07cf9e784810df7540
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/07/2019
ms.locfileid: "34769450"
---
# <a name="access-services-retirement"></a><span data-ttu-id="7a1c0-102">Piekļuves pakalpojumu pensijas</span><span class="sxs-lookup"><span data-stu-id="7a1c0-102">Access services retirement</span></span>

<span data-ttu-id="7a1c0-103">Kā mēs sākotnēji paziņoja, MC97576, martā 2017 un turpināja sazināties vairāk nekā pagājušajā gadā piekļuves pakalpojumiem ir pensijā, no Office 365.</span><span class="sxs-lookup"><span data-stu-id="7a1c0-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="7a1c0-104">Nākamais posms šajā procesā būs izņemšanas Access Web datu bāzes, kas izmanto SharePoint sarakstus kā to pamatā esošo datu krātuvi.</span><span class="sxs-lookup"><span data-stu-id="7a1c0-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="7a1c0-105">**Kā tas ietekmēs mani?**</span><span class="sxs-lookup"><span data-stu-id="7a1c0-105">**How does this affect me?**</span></span>

<span data-ttu-id="7a1c0-106">Sākot no jūnija 2019, mēs pieturas izveidi jaunās Access datu bāzēs, SharePoint Online un jāslēdz pakalpojumu un visus pārējos apps aprīlī 2020.</span><span class="sxs-lookup"><span data-stu-id="7a1c0-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="7a1c0-107">**Kas man jādara, lai sagatavotos šīs izmaiņas?**</span><span class="sxs-lookup"><span data-stu-id="7a1c0-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="7a1c0-108">Mēs iesakām jums izveidot pārejas plānu, jūsu organizāciju Access web datu bāzēm.</span><span class="sxs-lookup"><span data-stu-id="7a1c0-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="7a1c0-109">Admins var izmantot [SharePoint piekļuves app skeneris](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) iegūst piekļūt progr, ka vietas ir, izmantojot inventarizāciju.</span><span class="sxs-lookup"><span data-stu-id="7a1c0-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span> 

<span data-ttu-id="7a1c0-110">Ir vairāki veidi, kā Access web datu bāzes datu migrēšana:</span><span class="sxs-lookup"><span data-stu-id="7a1c0-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="7a1c0-111">Importēšanu, vietējo Access datu bāzē (. ACCDB) vai Excel failu.</span><span class="sxs-lookup"><span data-stu-id="7a1c0-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="7a1c0-112">Mēs arī iesakām izpētīt Microsoft PowerApps kā alternatīva platforma izveidošanai bezkoda business solutions web un mobilo ierīču palīdzību.</span><span class="sxs-lookup"><span data-stu-id="7a1c0-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>