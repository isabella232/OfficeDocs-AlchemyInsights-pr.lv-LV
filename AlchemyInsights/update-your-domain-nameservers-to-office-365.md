---
title: Atjauniniet savu domēna nameservers norādīt uz Microsoft
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: b49ca9422f582f906fc6c108c85cc26150474548
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720000"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="64088-102">Atjauniniet savu domēna nameservers norādīt uz Microsoft</span><span class="sxs-lookup"><span data-stu-id="64088-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="64088-103">Piezīme. Nosaukumu servera izmaiņu izplatīšanai dažkārt ir nepieciešams līdz pat 48 stundām ilgs laiks.</span><span class="sxs-lookup"><span data-stu-id="64088-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="64088-104">Lai iestatītu domēnu, izmantojot Microsoft, jūsu reģistratoram ir jāatjaunina nameservers.</span><span class="sxs-lookup"><span data-stu-id="64088-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="64088-105">Izveidojiet vai rediģējiet nosaukumu servera ierakstus savā domēnu reģistrētājā.</span><span class="sxs-lookup"><span data-stu-id="64088-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="64088-106">Dodieties uz domēnu reģistrētāja tīmekļa vietni un atrodiet apgabalu, kurā varat rediģēt nosaukumu serverus.</span><span class="sxs-lookup"><span data-stu-id="64088-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="64088-107">Izveidojiet vai rediģējiet divus nosaukumu servera ierakstus atbilstoši šādām vērtībām:</span><span class="sxs-lookup"><span data-stu-id="64088-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="64088-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="64088-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="64088-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="64088-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="64088-110">Saglabājiet izmaiņas.</span><span class="sxs-lookup"><span data-stu-id="64088-110">Save changes.</span></span>

<span data-ttu-id="64088-111">Varat arī atrast detalizētas instrukcijas šajā rakstā: [mainīt nameservers iestatīt Microsoft 365 ar jebkuru domēna reģistrētājs](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="64088-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  