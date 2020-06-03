---
title: Nosaukumu serveru maiņa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: f295e0d7872a13cf47e386343b159e51bc0504de
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508095"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="94986-102">Domēnu nosaukumu serveru atjaunināšana, lai norādītu uz Microsoft</span><span class="sxs-lookup"><span data-stu-id="94986-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="94986-103">Piezīme. Nosaukumu servera izmaiņu izplatīšanai dažkārt ir nepieciešams līdz pat 48 stundām ilgs laiks.</span><span class="sxs-lookup"><span data-stu-id="94986-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="94986-104">Lai iestatītu savu domēnu pakalpojumā Microsoft 365, pie domēnu reģistrētāja ir jāatjaunina nosaukumu serveri.</span><span class="sxs-lookup"><span data-stu-id="94986-104">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="94986-105">Izveidojiet vai rediģējiet nosaukumu servera ierakstus savā domēnu reģistrētājā.</span><span class="sxs-lookup"><span data-stu-id="94986-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="94986-106">Dodieties uz domēnu reģistrētāja tīmekļa vietni un atrodiet apgabalu, kurā varat rediģēt nosaukumu serverus.</span><span class="sxs-lookup"><span data-stu-id="94986-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="94986-107">Izveidojiet vai rediģējiet divus nosaukumu servera ierakstus atbilstoši šādām vērtībām:</span><span class="sxs-lookup"><span data-stu-id="94986-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="94986-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="94986-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="94986-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="94986-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="94986-110">Saglabājiet izmaiņas.</span><span class="sxs-lookup"><span data-stu-id="94986-110">Save changes.</span></span>

<span data-ttu-id="94986-111">Detalizētas instrukcijas skatiet šajā rakstā: [Nosaukumu serveru maiņa pie jebkura domēnu reģistrētāja](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="94986-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  