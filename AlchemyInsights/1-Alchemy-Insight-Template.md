---
title: 'Tāpat kā nosaukums ir labākais [KĀRTULA #-apraksts]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 1bb1cb35f06e16a2dc85b7e2642b9fa0d203945e
ms.sourcegitcommit: b032c2ac45540b1eb5dd68a4ec7ce1a5d6922f0e
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/30/2019
ms.locfileid: "29662937"
---
# <a name="required-customer-facing-h1-h2-doesnt-work"></a><span data-ttu-id="9c355-102">Doesn't darbu nepieciešamo klientu vērsts H1, H2</span><span class="sxs-lookup"><span data-stu-id="9c355-102">Required Customer Facing H1, H2 doesn't work</span></span>
<span data-ttu-id="9c355-103">Teksta piemērs bloķēt - izpildiet šos norādījumus:</span><span class="sxs-lookup"><span data-stu-id="9c355-103">Example text block - follow these instructions:</span></span>

1. <span data-ttu-id="9c355-104">Failus mapē **AlchemyInsights** vajadzētu būt kārtulas ID un kārtulas nosaukumā no [alķīmijas partneru portāla](https://alchemyportal.azurewebsites.net) nosaukums.</span><span class="sxs-lookup"><span data-stu-id="9c355-104">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="9c355-p101">ex. ***976-How-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="9c355-p101">ex. ***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="9c355-p102">Kā veidnei metadatus izmantotu šī faila sākumā. Nekas cits nav vajadzīgs.</span><span class="sxs-lookup"><span data-stu-id="9c355-p102">Use the metadata at the top of this file as your template. Nothing else is required.</span></span>
1. <span data-ttu-id="9c355-109">[Alchemy partneru portāla](https://alchemyportal.azurewebsites.net)virzītos uz leju līdz sadaļai **klientu ieskatu nosaukums:** un izmantot šo kā sākuma punkts H1 titra par ieskatu.</span><span class="sxs-lookup"><span data-stu-id="9c355-109">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="9c355-p103">Alķīmijas atziņas ir jābūt tikai vienu H1 augšpusē vai viņi pārtrauks ražošanu. H2s nepadara tik lietot **treknraksta** vai citām konvencijām neizsaka atsevišķās sekcijās.</span><span class="sxs-lookup"><span data-stu-id="9c355-p103">Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="9c355-112">Pēc tam aizpildiet pamattekstu, izmantojot iesaukumam Alchemy noteikums lapas sadaļā klientu atziņas</span><span class="sxs-lookup"><span data-stu-id="9c355-112">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="9c355-113">Aizzīmētiem sarakstiem ir smalka</span><span class="sxs-lookup"><span data-stu-id="9c355-113">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="9c355-114">Numurētus sarakstus pārāk</span><span class="sxs-lookup"><span data-stu-id="9c355-114">Numbered lists too</span></span>
    1. <span data-ttu-id="9c355-115">**Treknraksts** un *kursīvs* , tiek a-ok</span><span class="sxs-lookup"><span data-stu-id="9c355-115">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="9c355-116">Saites, vienmēr ir jābūt vai nu **"uz web saites" / ārējo** vai **dziļas saites uz lietotāja interfeisa elementus**, nevis iekšējās saites.</span><span class="sxs-lookup"><span data-stu-id="9c355-116">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="9c355-p104">Un tas tiešām jau ir mazliet pārāk ilgi. Vislabākā prakse ir apmēram 400 rakstzīmēm--</span><span class="sxs-lookup"><span data-stu-id="9c355-p104">And this is really already a bit too long. Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="9c355-p105">Kad jūsu lapa ir gatava, izvelciet to dzīvu zaru. Pēc tam [Alchemy partneru portālā](https://alchemyportal.azurewebsites.net) un url laukā ievadiet faila nosaukumu. Pārliecinieties, vai ieskatu pārskatīja un publicēts saka "Jā" un pēc tam noklikšķiniet uz atjaunināt kārtulu. (Tas izskatīsies skaistākas jaunajā versijā portālā - atbrīvojot drīz.)</span><span class="sxs-lookup"><span data-stu-id="9c355-p105">Once your content is ready, pull it to the live branch. Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field. Make sure Insight reviewed and published says "yes" and then click Update Rule. (This will look prettier in the new version of the portal - releasing soon.)</span></span>

![URL laukā](media/for-content-team.PNG)

