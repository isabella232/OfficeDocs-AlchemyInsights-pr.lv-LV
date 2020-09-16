---
title: Vietnes izveide pakalpojumā SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732238"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="47818-102">SharePoint vietņu izveide, izmantojot veidnes</span><span class="sxs-lookup"><span data-stu-id="47818-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="47818-103">Iespēja saglabāt vietni kā veidni netiek atbalstīta modernās saziņas vai grupas vietnēs.</span><span class="sxs-lookup"><span data-stu-id="47818-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="47818-104">Papildinformāciju par veidņu izmantošanu skatiet rakstā [SharePoint vietnes saglabāšana, lejupielāde un augšupielāde veidnes](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template)formātā.</span><span class="sxs-lookup"><span data-stu-id="47818-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="47818-105">Tālāk ir sniegtas dažas bieži sastopamas problēmas/risinājumi attiecībā uz vietnes vai saraksta saglabāšanu veidnes formātā pakalpojumā SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="47818-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="47818-106">**Poga saglabāt vietnes/saraksta veidni nav pieejama vai trūkst**</span><span class="sxs-lookup"><span data-stu-id="47818-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="47818-107">Administratoriem ir jāatļauj pielāgot skriptu, lai iespējotu veidnes līdzekļus.</span><span class="sxs-lookup"><span data-stu-id="47818-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="47818-108">Detalizētus norādījumus par piemēriem un apsvērumiem skatiet rakstā</span><span class="sxs-lookup"><span data-stu-id="47818-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="47818-109">Pielāgota skripta atļaušana vai aizliegšana</span><span class="sxs-lookup"><span data-stu-id="47818-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="47818-110">Komanda Saglabāt vietni kā veidni netiek atbalstīta, un tā var izraisīt problēmas vietnēs, kurās tiek izmantota SharePoint Server publicēšanas infrastruktūra.</span><span class="sxs-lookup"><span data-stu-id="47818-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="47818-111">**Vietnes veidni nevar izveidot vai tā nedarbojas pareizi**</span><span class="sxs-lookup"><span data-stu-id="47818-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="47818-112">Veidnei, iespējams, trūkst [līdzekļa](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) , un tā netiek aktivizēta.</span><span class="sxs-lookup"><span data-stu-id="47818-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="47818-113">Ja šis līdzeklis nav pieejams aktivizēšanai pašreizējā vietņu kolekcijā, vietnes veidni nevar izmantot, lai izveidotu vietni.</span><span class="sxs-lookup"><span data-stu-id="47818-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="47818-114">Pārbaudiet, vai kāds saraksts vai bibliotēka pārsniedz [saraksta skata ierobežojuma slieksni](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 vienumiem, jo tas var bloķēt vietnes veidnes izveidi.</span><span class="sxs-lookup"><span data-stu-id="47818-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="47818-115">Vietne, iespējams, izmanto pārāk daudz resursu, tāpēc vietnes veidne pārsniedz 50 MB ierobežojumu.</span><span class="sxs-lookup"><span data-stu-id="47818-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="47818-116">Pastāv problēmas, kas rāda datus no saraksta, kas izmanto uzmeklēšanas kolonnu.</span><span class="sxs-lookup"><span data-stu-id="47818-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="47818-117">Lai iegūtu papildinformāciju, skatiet rakstu [veidnes ģenerētie saraksti nerāda datus no pareiza uzmeklēšanas saraksta pakalpojumā SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="47818-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="47818-118">Lai iegūtu detalizētāku informāciju par biežāk sastopamajām problēmām un risinājumiem, skatiet [lapu veidņu izveide un lietošana](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="47818-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



