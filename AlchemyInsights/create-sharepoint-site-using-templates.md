---
title: Izveidot vietni SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b9009fdbdc2a5e7443151446daade1685d2f5d45
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770430"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="fdbd6-102">SharePoint vietņu izveide, izmantojot veidnes</span><span class="sxs-lookup"><span data-stu-id="fdbd6-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="fdbd6-103">Iespēja saglabāt vietni kā veidni netiek atbalstīta mūsdienu saziņas vai grupas vietnēs.</span><span class="sxs-lookup"><span data-stu-id="fdbd6-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="fdbd6-104">Lai iegūtu papildinformāciju par veidņu lietošanu, skatiet sadaļu [SharePoint vietnes kā veidnes saglabāšana, lejupielāde un augšupielāde](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span><span class="sxs-lookup"><span data-stu-id="fdbd6-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="fdbd6-105">Tālāk ir norādītas dažas bieži sastopamas problēmas/risinājumi attiecībā uz vietnes vai saraksta saglabāšanu kā veidni programmā SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="fdbd6-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="fdbd6-106">**Poga saglabāt vietnes/saraksta veidni nav pieejama vai tās trūkst**</span><span class="sxs-lookup"><span data-stu-id="fdbd6-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="fdbd6-107">Administratoriem ir jāatļauj pielāgots skripts, lai iespējotu veidnes līdzekļus.</span><span class="sxs-lookup"><span data-stu-id="fdbd6-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="fdbd6-108">Detalizētus soļus, piemērus un apsvērumus sk.</span><span class="sxs-lookup"><span data-stu-id="fdbd6-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="fdbd6-109">Atļaut vai aizliegt pielāgotu skriptu</span><span class="sxs-lookup"><span data-stu-id="fdbd6-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="fdbd6-110">Saglabāt vietni kā veidni komanda netiek atbalstīta un var radīt problēmas vietnēs, kas izmanto SharePoint Server publicēšanas infrastruktūra.</span><span class="sxs-lookup"><span data-stu-id="fdbd6-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="fdbd6-111">**Vietnes veidni nevar izveidot vai tā nedarbojas pareizi**</span><span class="sxs-lookup"><span data-stu-id="fdbd6-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="fdbd6-112">Iespējams, ka veidnei trūkst [līdzekļa](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) , un tā netiks aktivizēta.</span><span class="sxs-lookup"><span data-stu-id="fdbd6-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="fdbd6-113">Ja līdzeklis nav pieejams, lai aktivizētu pašreizējā vietņu kolekcijā, vietnes veidni nevar izmantot, lai izveidotu vietni.</span><span class="sxs-lookup"><span data-stu-id="fdbd6-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="fdbd6-114">Pārbaudiet, vai kādi saraksti vai bibliotēkas pārsniedz [saraksta skata ierobežojuma slieksnis](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 vienumus, jo tas var bloķēt vietnes veidnes izveide.</span><span class="sxs-lookup"><span data-stu-id="fdbd6-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="fdbd6-115">Vietne var izmantot pārāk daudz resursu un tādēļ vietnes veidne pārsniedz 50 MB ierobežojumu.</span><span class="sxs-lookup"><span data-stu-id="fdbd6-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="fdbd6-116">Ir problēmas, parādot datus no saraksta, kas izmanto uzmeklēšanas kolonnu.</span><span class="sxs-lookup"><span data-stu-id="fdbd6-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="fdbd6-117">Lai iegūtu papildinformāciju, skatiet [veidne ģenerēts saraksts netiek parādīts datus no pareizā uzmeklēšanas saraksta SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="fdbd6-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="fdbd6-118">Sīkāku informāciju par kopīgām problēmām un risinājumiem, lūdzu, pārbaudiet [izveidot un izmantot vietnes veidnes](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="fdbd6-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



