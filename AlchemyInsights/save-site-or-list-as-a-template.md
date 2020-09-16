---
title: Vietnes vai saraksta saglabāšana veidnes formātā
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727538"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="9dc4c-102">Vietnes vai saraksta saglabāšana veidnes formātā</span><span class="sxs-lookup"><span data-stu-id="9dc4c-102">Save site or list as a template</span></span>

<span data-ttu-id="9dc4c-103">SharePoint vietnes veidnes ir iepriekš izveidotas definīcijas, kas paredzētas noteiktai biznesa nepieciešamībai.</span><span class="sxs-lookup"><span data-stu-id="9dc4c-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="9dc4c-104">Papildinformāciju skatiet rakstā [veidņu izmantošana, lai izveidotu dažādu veidu SharePoint vietnes](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="9dc4c-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="9dc4c-105">Tālāk ir sniegtas dažas bieži sastopamas problēmas/risinājumi attiecībā uz vietnes vai saraksta saglabāšanu veidnes formātā pakalpojumā SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="9dc4c-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="9dc4c-106">**Poga saglabāt vietnes/saraksta veidni nav pieejama vai trūkst**.</span><span class="sxs-lookup"><span data-stu-id="9dc4c-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="9dc4c-107">Administratoriem ir jāatļauj pielāgot skriptu, lai iespējotu veidnes līdzekļus.</span><span class="sxs-lookup"><span data-stu-id="9dc4c-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="9dc4c-108">Detalizētus norādījumus par piemēriem un apsvērumiem skatiet rakstā [pielāgota skripta atļaušana vai novēršana](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="9dc4c-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="9dc4c-109">Komanda Saglabāt vietni kā veidni netiek atbalstīta, un tā var izraisīt problēmas vietnēs, kurās tiek izmantota SharePoint Server publicēšanas infrastruktūra.</span><span class="sxs-lookup"><span data-stu-id="9dc4c-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="9dc4c-110">**Vietnes veidni nevar izveidot vai tā nedarbojas pareizi**</span><span class="sxs-lookup"><span data-stu-id="9dc4c-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="9dc4c-111">Veidnei, iespējams, trūkst [līdzekļa](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) , un tā netiek aktivizēta.</span><span class="sxs-lookup"><span data-stu-id="9dc4c-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="9dc4c-112">Ja šis līdzeklis nav pieejams aktivizēšanai pašreizējā vietņu kolekcijā, vietnes veidni nevar izmantot, lai izveidotu vietni.</span><span class="sxs-lookup"><span data-stu-id="9dc4c-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="9dc4c-113">Pārbaudiet, vai kāds saraksts vai bibliotēka pārsniedz [saraksta skata ierobežojuma slieksni](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 vienumiem, jo tas var bloķēt vietnes veidnes izveidi.</span><span class="sxs-lookup"><span data-stu-id="9dc4c-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="9dc4c-114">Vietne, iespējams, izmanto pārāk daudz resursu, tāpēc vietnes veidne pārsniedz 50 megabaitu (MB) ierobežojumu.</span><span class="sxs-lookup"><span data-stu-id="9dc4c-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="9dc4c-115">Pastāv problēmas, kas rāda datus no saraksta, kas izmanto uzmeklēšanas kolonnu.</span><span class="sxs-lookup"><span data-stu-id="9dc4c-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="9dc4c-116">Lai iegūtu papildinformāciju, skatiet rakstu [veidnes ģenerētie saraksti nerāda datus no pareiza uzmeklēšanas saraksta pakalpojumā SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="9dc4c-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="9dc4c-117">Detalizētāku informāciju par biežāk sastopamajām problēmām un risinājumiem skatiet sadaļā [vietņu veidņu izveide un lietošana](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="9dc4c-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

