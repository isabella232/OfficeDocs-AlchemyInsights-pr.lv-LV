---
title: Izveidot vietni, SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 7c24a0cf3bcae0f2780c1cb33c911cb38c1ca5cb
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/22/2019
ms.locfileid: "36515005"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="99fc6-102">Izveidojiet SharePoint vietnes, izmantojot veidnes</span><span class="sxs-lookup"><span data-stu-id="99fc6-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="99fc6-103">SharePoint vietņu veidnes ir iebūvētām definīcijas, kas paredzēta ap konkrētu biznesa vajadzību.</span><span class="sxs-lookup"><span data-stu-id="99fc6-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="99fc6-104">Plašāku informāciju skatiet [izmantojot veidnes, lai radītu dažādu veidu SharePoint vietnēs](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="99fc6-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="99fc6-105">Šeit ir dažas kopējas problēmas/risinājumi attiecībā uz saglabāšanas vietu vai sarakstu kā veidni Sharepoint Online.</span><span class="sxs-lookup"><span data-stu-id="99fc6-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="99fc6-106">**Saglabāt sarakstā un vietnes veidnes poga nav pieejama vai trūkst**</span><span class="sxs-lookup"><span data-stu-id="99fc6-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="99fc6-107">Administratoriem būs nepieciešams pielāgots skripts ļauj iespējot veidnes līdzekļi.</span><span class="sxs-lookup"><span data-stu-id="99fc6-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="99fc6-108">Detalizēts darbības piemērus un apsvērumi skatiet</span><span class="sxs-lookup"><span data-stu-id="99fc6-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="99fc6-109">Atļautu vai aizliegtu pielāgots skripts</span><span class="sxs-lookup"><span data-stu-id="99fc6-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="99fc6-110">Saglabāt vietni kā veidni komanda netiek atbalstīta, un var radīt problēmas uz vietām, kas izmanto SharePoint Server publicēšanas infrastruktūru.</span><span class="sxs-lookup"><span data-stu-id="99fc6-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="99fc6-111">**Vietnes veidne nevar izveidot vai nedarbojas pareizi**</span><span class="sxs-lookup"><span data-stu-id="99fc6-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="99fc6-112">Veidni var trūkt [līdzekli](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) un nevar aktivizēt.</span><span class="sxs-lookup"><span data-stu-id="99fc6-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="99fc6-113">Ja šī funkcija nav pieejama, lai aktivizētu vietņu kolekcijā, vietnes veidne nevar izmantot, lai izveidotu vietni.</span><span class="sxs-lookup"><span data-stu-id="99fc6-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="99fc6-114">Pārbaudiet, lai redzētu, ja nevienu sarakstu vai bibliotēku pārsniegt 5000 vienumus [Saraksta skats ierobežojuma slieksni](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) , jo tas var bloķēt vietnes veidnes izveide.</span><span class="sxs-lookup"><span data-stu-id="99fc6-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="99fc6-115">Vietne, iespējams, izmanto pārāk daudz resursu un tādēļ vietņu veidņu pārsniedz 50 MB.</span><span class="sxs-lookup"><span data-stu-id="99fc6-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="99fc6-116">Pastāv problēmas attēlot datus no saraksta, kas izmanto uzmeklēšanas kolonnu.</span><span class="sxs-lookup"><span data-stu-id="99fc6-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="99fc6-117">Papildinformāciju skatiet sadaļā [veidnes ģenerēts saraksts neparādās dati no SharePoint Online pareizo meklēšanas sarakstā](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="99fc6-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>

<span data-ttu-id="99fc6-118">Sīkāka informācija par kopīgu problēmu un risinājumu, lūdzu, pārbaudiet [vietnes veidņu izveidošana un izmantošana](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="99fc6-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



