---
title: Nosaukumu serveru maiņa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 67680a6fa514d31ccb88cc8691a199cd1f58a402
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818619"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="ffdb3-102">Domēnu nosaukumu serveru atjaunināšana, lai norādītu uz Microsoft</span><span class="sxs-lookup"><span data-stu-id="ffdb3-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="ffdb3-103">Piezīme. Nosaukumu servera izmaiņu izplatīšanai dažkārt ir nepieciešams līdz pat 48 stundām ilgs laiks.</span><span class="sxs-lookup"><span data-stu-id="ffdb3-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="ffdb3-104">Lai iestatītu savu domēnu pakalpojumā Microsoft 365, pie domēnu reģistrētāja ir jāatjaunina nosaukumu serveri.</span><span class="sxs-lookup"><span data-stu-id="ffdb3-104">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="ffdb3-105">Izveidojiet vai rediģējiet nosaukumu servera ierakstus savā domēnu reģistrētājā.</span><span class="sxs-lookup"><span data-stu-id="ffdb3-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="ffdb3-106">Dodieties uz domēnu reģistrētāja tīmekļa vietni un atrodiet apgabalu, kurā varat rediģēt nosaukumu serverus.</span><span class="sxs-lookup"><span data-stu-id="ffdb3-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="ffdb3-107">Izveidojiet vai rediģējiet divus nosaukumu servera ierakstus atbilstoši šādām vērtībām:</span><span class="sxs-lookup"><span data-stu-id="ffdb3-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="ffdb3-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="ffdb3-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="ffdb3-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="ffdb3-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="ffdb3-110">Saglabājiet izmaiņas.</span><span class="sxs-lookup"><span data-stu-id="ffdb3-110">Save changes.</span></span>

<span data-ttu-id="ffdb3-111">Detalizētas instrukcijas skatiet šajā rakstā: [Nosaukumu serveru maiņa pie jebkura domēnu reģistrētāja](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="ffdb3-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  