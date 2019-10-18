---
title: Nosaukumu serveru maiņa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 51532f42e7cbd39ebad3f0160465218c6e1454a2
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736656"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="076a9-102">Domēnu nosaukumu serveru atjaunināšana uz Office 365</span><span class="sxs-lookup"><span data-stu-id="076a9-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="076a9-103">Piezīme. Nosaukumu servera izmaiņu izplatīšanai dažkārt ir nepieciešams līdz pat 48 stundām ilgs laiks.</span><span class="sxs-lookup"><span data-stu-id="076a9-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="076a9-104">Lai iestatītu savu domēnu pakalpojumā Office 365, domēnu reģistrētājā ir jāatjaunina nosaukumu serveri.</span><span class="sxs-lookup"><span data-stu-id="076a9-104">To set up your domain in Office 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="076a9-105">Izveidojiet vai rediģējiet nosaukumu servera ierakstus savā domēnu reģistrētājā.</span><span class="sxs-lookup"><span data-stu-id="076a9-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="076a9-106">Dodieties uz domēnu reģistrētāja tīmekļa vietni un atrodiet apgabalu, kurā varat rediģēt nosaukumu serverus.</span><span class="sxs-lookup"><span data-stu-id="076a9-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="076a9-107">Izveidojiet vai rediģējiet divus nosaukumu servera ierakstus atbilstoši šādām vērtībām:</span><span class="sxs-lookup"><span data-stu-id="076a9-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="076a9-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="076a9-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="076a9-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="076a9-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="076a9-110">Saglabājiet izmaiņas.</span><span class="sxs-lookup"><span data-stu-id="076a9-110">Save changes.</span></span>

<span data-ttu-id="076a9-111">Detalizētas instrukcijas skatiet šajā rakstā: [Nosaukumu serveru maiņa, lai iestatītu Office 365 jebkurā domēnu reģistrētājā](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="076a9-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  