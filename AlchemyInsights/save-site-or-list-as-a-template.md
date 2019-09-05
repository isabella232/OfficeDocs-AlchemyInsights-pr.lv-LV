---
title: Saglabāt vietni vai sarakstu kā veidni
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 1fe0a2f5bf65ef4e8cabf3d05a701c8eff966435
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752039"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="2bf73-102">Saglabāt vietni vai sarakstu kā veidni</span><span class="sxs-lookup"><span data-stu-id="2bf73-102">Save site or list as a template</span></span>

<span data-ttu-id="2bf73-103">SharePoint vietnes veidnes ir iepriekš izveidotas definīcijas, kas izstrādātas ap konkrētu biznesa vajadzību.</span><span class="sxs-lookup"><span data-stu-id="2bf73-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="2bf73-104">Papildinformāciju skatiet sadaļā [veidņu lietošana, lai izveidotu dažādu veidu SharePoint vietnes](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="2bf73-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="2bf73-105">Tālāk ir norādītas dažas bieži sastopamas problēmas/risinājumi attiecībā uz vietnes vai saraksta saglabāšanu kā veidni programmā SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="2bf73-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="2bf73-106">**Poga saglabāt vietnes/saraksta veidni nav pieejama vai tās trūkst**.</span><span class="sxs-lookup"><span data-stu-id="2bf73-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="2bf73-107">Administratoriem ir jāatļauj pielāgots skripts, lai iespējotu veidnes līdzekļus.</span><span class="sxs-lookup"><span data-stu-id="2bf73-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="2bf73-108">Detalizētas darbības, piemērus un apsvērumus skatiet sadaļā [Atļaut vai aizliegt pielāgotu skriptu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="2bf73-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="2bf73-109">Saglabāt vietni kā veidni komanda netiek atbalstīta un var radīt problēmas vietnēs, kas izmanto SharePoint Server publicēšanas infrastruktūra.</span><span class="sxs-lookup"><span data-stu-id="2bf73-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="2bf73-110">**Vietnes veidni nevar izveidot vai tā nedarbojas pareizi**</span><span class="sxs-lookup"><span data-stu-id="2bf73-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="2bf73-111">Iespējams, ka veidnei trūkst [līdzekļa](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) , un tā netiks aktivizēta.</span><span class="sxs-lookup"><span data-stu-id="2bf73-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="2bf73-112">Ja līdzeklis nav pieejams, lai aktivizētu pašreizējā vietņu kolekcijā, vietnes veidni nevar izmantot, lai izveidotu vietni.</span><span class="sxs-lookup"><span data-stu-id="2bf73-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="2bf73-113">Pārbaudiet, vai kādi saraksti vai bibliotēkas pārsniedz [saraksta skata ierobežojuma slieksnis](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 vienumus, jo tas var bloķēt vietnes veidnes izveide.</span><span class="sxs-lookup"><span data-stu-id="2bf73-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="2bf73-114">Iespējams, ka vietne izmanto pārāk daudz resursu, tāpēc vietnes veidne pārsniedz 50 megabaitu (MB) ierobežojumu.</span><span class="sxs-lookup"><span data-stu-id="2bf73-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="2bf73-115">Ir problēmas, parādot datus no saraksta, kas izmanto uzmeklēšanas kolonnu.</span><span class="sxs-lookup"><span data-stu-id="2bf73-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="2bf73-116">Lai iegūtu papildinformāciju, skatiet [veidne ģenerēts saraksts netiek parādīts datus no pareizā uzmeklēšanas saraksta SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="2bf73-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="2bf73-117">Sīkāku informāciju par kopīgām problēmām un risinājumiem, lūdzu, norādi, [izveidot un izmantot vietnes veidnes](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="2bf73-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

