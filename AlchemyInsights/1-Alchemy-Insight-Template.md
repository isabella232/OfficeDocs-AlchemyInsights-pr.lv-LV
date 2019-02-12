---
title: 'Tāpat kā nosaukums ir labākais [KĀRTULA #-apraksts]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 01d8b03209e734f1218de61d964524b1b9e1d044
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/12/2019
ms.locfileid: "29939305"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="d7288-102">Vajadzīga alķīmija Header H1, H2 ir nestrādā.</span><span class="sxs-lookup"><span data-stu-id="d7288-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="d7288-103">Labāko praksi un pamatnostādnēm par alķīmiju autorēšanas:</span><span class="sxs-lookup"><span data-stu-id="d7288-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="d7288-p101">**Neligzdo Alchemy atziņas mapēs**- tas saplīst url struktūru. Mēs meklēja šo noteikšanu.</span><span class="sxs-lookup"><span data-stu-id="d7288-p101">**Do not nest Alchemy Insights in folders**- this will break the url structure. We're looking into fixing this.</span></span>
1. <span data-ttu-id="d7288-106">Failus mapē **AlchemyInsights** vajadzētu būt kārtulas ID un kārtulas nosaukumā no [alķīmijas partneru portāla](https://alchemyportal.azurewebsites.net) nosaukums.</span><span class="sxs-lookup"><span data-stu-id="d7288-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="d7288-p102">ex. ***976-How-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="d7288-p102">ex. ***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="d7288-p103">Kā veidnei metadatus izmantotu šī faila sākumā. Nekas cits nav vajadzīgs.</span><span class="sxs-lookup"><span data-stu-id="d7288-p103">Use the metadata at the top of this file as your template. Nothing else is required.</span></span>
1. <span data-ttu-id="d7288-111">[Alchemy partneru portāla](https://alchemyportal.azurewebsites.net)virzītos uz leju līdz sadaļai **klientu ieskatu nosaukums:** un izmantot šo kā sākuma punkts H1 titra par ieskatu.</span><span class="sxs-lookup"><span data-stu-id="d7288-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="d7288-p104">Alķīmijas atziņas ir jābūt tikai vienu H1 augšpusē vai viņi pārtrauks ražošanu. H2s nepadara tik lietot **treknraksta** vai citām konvencijām neizsaka atsevišķās sekcijās.</span><span class="sxs-lookup"><span data-stu-id="d7288-p104">Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="d7288-114">Pēc tam aizpildiet pamattekstu, izmantojot iesaukumam Alchemy noteikums lapas sadaļā klientu atziņas</span><span class="sxs-lookup"><span data-stu-id="d7288-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="d7288-115">Aizzīmētiem sarakstiem ir smalka</span><span class="sxs-lookup"><span data-stu-id="d7288-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="d7288-116">Numurētus sarakstus pārāk</span><span class="sxs-lookup"><span data-stu-id="d7288-116">Numbered lists too</span></span>
    1. <span data-ttu-id="d7288-117">**Treknraksts** un *kursīvs* , tiek a-ok</span><span class="sxs-lookup"><span data-stu-id="d7288-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="d7288-118">Saites, vienmēr ir jābūt vai nu **"uz web saites" / ārējo** vai **dziļas saites uz lietotāja interfeisa elementus**, nevis iekšējās saites.</span><span class="sxs-lookup"><span data-stu-id="d7288-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="d7288-p105">Un tas tiešām jau ir mazliet pārāk ilgi. Vislabākā prakse ir apmēram 400 rakstzīmēm--</span><span class="sxs-lookup"><span data-stu-id="d7288-p105">And this is really already a bit too long. Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="d7288-p106">Kad jūsu lapa ir gatava, izvelciet to dzīvu zaru. Pēc tam [Alchemy partneru portālā](https://alchemyportal.azurewebsites.net) un url laukā ievadiet faila nosaukumu. Pārliecinieties, vai ieskatu pārskatīja un publicēts saka "Jā" un pēc tam noklikšķiniet uz atjaunināt kārtulu. **(Tas izskatīsies skaistākas jaunajā versijā portālā - atbrīvojot drīz.)** 
 ![url laukā](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="d7288-p106">Once your content is ready, pull it to the live branch. Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field. Make sure Insight reviewed and published says "yes" and then click Update Rule. **(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

