---
title: Piekļuves pakalpojumu pensijas
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 8886d7a6fad49e942e17f6a2f3c98542f87aae0b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/22/2019
ms.locfileid: "36495758"
---
# <a name="access-services-retirement"></a><span data-ttu-id="79189-102">Piekļuves pakalpojumu pensijas</span><span class="sxs-lookup"><span data-stu-id="79189-102">Access services retirement</span></span>

<span data-ttu-id="79189-103">Kā mēs sākotnēji paziņoja, MC97576, martā 2017 un turpināja sazināties vairāk nekā pagājušajā gadā piekļuves pakalpojumiem ir pensijā, no Office 365.</span><span class="sxs-lookup"><span data-stu-id="79189-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="79189-104">Nākamais posms šajā procesā būs izņemšanas Access Web datu bāzes, kas izmanto SharePoint sarakstus kā to pamatā esošo datu krātuvi.</span><span class="sxs-lookup"><span data-stu-id="79189-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="79189-105">**Kā tas ietekmēs mani?**</span><span class="sxs-lookup"><span data-stu-id="79189-105">**How does this affect me?**</span></span>

<span data-ttu-id="79189-106">Sākot no jūnija 2019, mēs pieturas izveidi jaunās Access datu bāzēs, SharePoint Online un jāslēdz pakalpojumu un visus pārējos apps aprīlī 2020.</span><span class="sxs-lookup"><span data-stu-id="79189-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="79189-107">**Kas man jādara, lai sagatavotos šīs izmaiņas?**</span><span class="sxs-lookup"><span data-stu-id="79189-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="79189-108">Mēs iesakām jums izveidot pārejas plānu, jūsu organizāciju Access web datu bāzēm.</span><span class="sxs-lookup"><span data-stu-id="79189-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="79189-109">Admins var izmantot [SharePoint piekļuves app skeneris](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) iegūst piekļūt progr, ka vietas ir, izmantojot inventarizāciju.</span><span class="sxs-lookup"><span data-stu-id="79189-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="79189-110">Ir vairāki veidi, kā Access web datu bāzes datu migrēšana:</span><span class="sxs-lookup"><span data-stu-id="79189-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="79189-111">Importēšanu, vietējo Access datu bāzē (. ACCDB) vai Excel failu.</span><span class="sxs-lookup"><span data-stu-id="79189-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="79189-112">Mēs arī iesakām izpētīt Microsoft PowerApps kā alternatīva platforma izveidošanai bezkoda business solutions web un mobilo ierīču palīdzību.</span><span class="sxs-lookup"><span data-stu-id="79189-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>