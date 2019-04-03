---
title: Vietni vai sarakstu saglabātu kā veidni
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 7930551c0938501d006f791491594f9d6d9ba260
ms.sourcegitcommit: 56c52c73e752414d66785f175c3a0e2925ad41c1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/02/2019
ms.locfileid: "31044011"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="335e8-102">Vietni vai sarakstu saglabātu kā veidni</span><span class="sxs-lookup"><span data-stu-id="335e8-102">Save site or list as a template</span></span>

<span data-ttu-id="335e8-103">SharePoint vietņu veidnes ir iebūvētām definīcijas, kas paredzēta ap konkrētu biznesa vajadzību.</span><span class="sxs-lookup"><span data-stu-id="335e8-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="335e8-104">Plašāku informāciju skatiet [izmantojot veidnes, lai radītu dažādu veidu SharePoint vietnēs](https://support.office.com/en-us/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="335e8-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/en-us/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="335e8-105">Šeit ir dažas kopējas problēmas/risinājumi attiecībā uz saglabāšanas vietu vai sarakstu kā veidni SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="335e8-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="335e8-106">**Saglabāt sarakstā un vietnes veidnes poga ir nav pieejama vai tās trūkst**.</span><span class="sxs-lookup"><span data-stu-id="335e8-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="335e8-107">Administratoriem būs nepieciešams pielāgots skripts ļauj iespējot veidnes līdzekļi.</span><span class="sxs-lookup"><span data-stu-id="335e8-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="335e8-108">Detalizētām darbībām, piemērus un apsvērumi sk [Atļaut vai aizliegt pielāgotu skriptu](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="335e8-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="335e8-109">Saglabāt vietni kā veidni komanda netiek atbalstīta, un var radīt problēmas uz vietām, kas izmanto SharePoint Server publicēšanas infrastruktūru.</span><span class="sxs-lookup"><span data-stu-id="335e8-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


**<span data-ttu-id="335e8-110">Vietnes veidne nevar izveidot vai nedarbojas pareizi</span><span class="sxs-lookup"><span data-stu-id="335e8-110">The site template cannot be created or does not work correctly</span></span>**

- <span data-ttu-id="335e8-111">Veidni var trūkt [līdzekli](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) un nevar aktivizēt.</span><span class="sxs-lookup"><span data-stu-id="335e8-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="335e8-112">Ja šī funkcija nav pieejama, lai aktivizētu vietņu kolekcijā, vietnes veidne nevar izmantot, lai izveidotu vietni.</span><span class="sxs-lookup"><span data-stu-id="335e8-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="335e8-113">Pārbaudiet, lai redzētu, ja nevienu sarakstu vai bibliotēku pārsniegt 5000 vienumus [Saraksta skats ierobežojuma slieksni](https://support.office.com/en-us/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) , jo tas var bloķēt vietnes veidnes izveide.</span><span class="sxs-lookup"><span data-stu-id="335e8-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/en-us/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="335e8-114">Vietne, iespējams, izmanto pārāk daudz resursu un tādēļ vietņu veidņu pārsniedz 50 megabaitu (MB) robežu.</span><span class="sxs-lookup"><span data-stu-id="335e8-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="335e8-115">Pastāv problēmas attēlot datus no saraksta, kas izmanto uzmeklēšanas kolonnu.</span><span class="sxs-lookup"><span data-stu-id="335e8-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="335e8-116">Papildinformāciju skatiet sadaļā [veidnes ģenerēts saraksts neparādās dati no SharePoint Online pareizo meklēšanas sarakstā](https://support.office.com/en-us/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="335e8-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://support.office.com/en-us/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>


<span data-ttu-id="335e8-117">Sīkāka informācija par bieži sastopamām problēmām un risinājumiem, lūdzu atsauci, [vietņu veidņu izveidošana un izmantošana](https://support.office.com/en-us/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="335e8-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/en-us/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

