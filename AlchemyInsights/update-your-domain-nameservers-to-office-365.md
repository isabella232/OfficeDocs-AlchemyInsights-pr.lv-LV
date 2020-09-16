---
title: Domēnu nosaukumu serveru atjaunināšana, lai norādītu uz Microsoft
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 7322fa640f6d043f057c8b7a5e06a18dcd10eec5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734918"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="ee0c0-102">Domēnu nosaukumu serveru atjaunināšana, lai norādītu uz Microsoft</span><span class="sxs-lookup"><span data-stu-id="ee0c0-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="ee0c0-103">Piezīme. Nosaukumu servera izmaiņu izplatīšanai dažkārt ir nepieciešams līdz pat 48 stundām ilgs laiks.</span><span class="sxs-lookup"><span data-stu-id="ee0c0-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="ee0c0-104">Lai iestatītu savu domēnu ar Microsoft, ir jāatjaunina jūsu reģistrētāja nosaukumu serveri.</span><span class="sxs-lookup"><span data-stu-id="ee0c0-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="ee0c0-105">Izveidojiet vai rediģējiet nosaukumu servera ierakstus savā domēnu reģistrētājā.</span><span class="sxs-lookup"><span data-stu-id="ee0c0-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="ee0c0-106">Dodieties uz domēnu reģistrētāja tīmekļa vietni un atrodiet apgabalu, kurā varat rediģēt nosaukumu serverus.</span><span class="sxs-lookup"><span data-stu-id="ee0c0-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="ee0c0-107">Izveidojiet vai rediģējiet divus nosaukumu servera ierakstus atbilstoši šādām vērtībām:</span><span class="sxs-lookup"><span data-stu-id="ee0c0-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="ee0c0-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="ee0c0-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="ee0c0-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="ee0c0-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="ee0c0-110">Saglabājiet izmaiņas.</span><span class="sxs-lookup"><span data-stu-id="ee0c0-110">Save changes.</span></span>

<span data-ttu-id="ee0c0-111">Detalizētus norādījumus skatiet šajā rakstā: [nosaukumu serveru maiņa, lai iestatītu Microsoft 365 ar jebkuru domēnu reģistrētāju](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="ee0c0-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  