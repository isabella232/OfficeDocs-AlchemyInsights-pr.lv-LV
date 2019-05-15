---
title: Piekļuves pakalpojumu pensijas
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 395dac6abf1562aa0da0b1d87eddd943affefc3f
ms.sourcegitcommit: b2c9202b94fa1ce73dbeb3e43b219ba07e46e7e3
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/14/2019
ms.locfileid: "33973932"
---
# <a name="access-services-retirement"></a><span data-ttu-id="00549-102">Piekļuves pakalpojumu pensijas</span><span class="sxs-lookup"><span data-stu-id="00549-102">Access services retirement</span></span>

<span data-ttu-id="00549-103">Kā mēs sākotnēji paziņoja, MC97576, martā 2017 un turpināja sazināties vairāk nekā pagājušajā gadā piekļuves pakalpojumiem ir pensijā, no Office 365.</span><span class="sxs-lookup"><span data-stu-id="00549-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="00549-104">Nākamais posms šajā procesā būs izņemšanas Access Web datu bāzes, kas izmanto SharePoint sarakstus kā to pamatā esošo datu krātuvi.</span><span class="sxs-lookup"><span data-stu-id="00549-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

## <a name="how-does-this-affect-me"></a><span data-ttu-id="00549-105">Kā tas ietekmēs mani?</span><span class="sxs-lookup"><span data-stu-id="00549-105">How does this affect me?</span></span>

<span data-ttu-id="00549-106">Sākot no jūnija 2019, mēs pieturas izveidi jaunās Access datu bāzēs, SharePoint Online un jāslēdz pakalpojumu un visus pārējos apps aprīlī 2020.</span><span class="sxs-lookup"><span data-stu-id="00549-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

## <a name="what-do-i-need-to-do-to-prepare-for-this-change"></a><span data-ttu-id="00549-107">Kas man jādara, lai sagatavotos šīs izmaiņas?</span><span class="sxs-lookup"><span data-stu-id="00549-107">What do I need to do to prepare for this change?</span></span>

<span data-ttu-id="00549-108">Mēs iesakām jums izveidot pārejas plānu, jūsu organizāciju Access web datu bāzēm.</span><span class="sxs-lookup"><span data-stu-id="00549-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="00549-109">Admins var izmantot [SharePoint piekļuves app skeneris](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) iegūst piekļūt progr, ka vietas ir, izmantojot inventarizāciju.</span><span class="sxs-lookup"><span data-stu-id="00549-109">Admins can use the [SharePoint Access app scanner](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) to obtain an inventory of the Access apps that sites are using.</span></span> 

<span data-ttu-id="00549-110">Ir vairāki veidi, kā Access web datu bāzes datu migrēšana:</span><span class="sxs-lookup"><span data-stu-id="00549-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="00549-111">Importēšanu, vietējo Access datu bāzē (. ACCDB) vai Excel failu.</span><span class="sxs-lookup"><span data-stu-id="00549-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="00549-112">Mēs arī iesakām izpētīt Microsoft PowerApps kā alternatīva platforma izveidošanai bezkoda business solutions web un mobilo ierīču palīdzību.</span><span class="sxs-lookup"><span data-stu-id="00549-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>