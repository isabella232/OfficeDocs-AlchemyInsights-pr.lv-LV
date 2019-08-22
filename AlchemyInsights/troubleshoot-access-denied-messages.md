---
title: Novērst problēmas ziņojumu piekļuve liegta
ms.author: kaarins
author: kaarins
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: e4fea7188bd77ba876e2a245414372c3ff836059
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/22/2019
ms.locfileid: "36500418"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="37f20-102">Novērst problēmas ziņojumu piekļuve liegta</span><span class="sxs-lookup"><span data-stu-id="37f20-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="37f20-103">Ja kāds got "Piekļuve liegta" ziņojuma izveidotu par koplietojamu mapi SharePoint, vietņu kolekcijas administrators, iespējams, ir iespējota "ierobežota piekļuve lietotāja atļauju lockdown režīms."</span><span class="sxs-lookup"><span data-stu-id="37f20-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="37f20-104">Lai izslēgtu šo opciju:</span><span class="sxs-lookup"><span data-stu-id="37f20-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="37f20-105">Atrodiet vietni, noklikšķiniet uz ikonas iestatījumus un pēc tam noklikšķiniet uz **Vietnes iestatījumi**.</span><span class="sxs-lookup"><span data-stu-id="37f20-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="37f20-106">Sadaļā **Vietņu kolekcijas administrators**, noklikšķiniet uz **vietņu kolekcijas līdzekļus**.</span><span class="sxs-lookup"><span data-stu-id="37f20-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="37f20-107">Blakus **ierobežotu piekļuvi lietotāja atļauju slēgts režīmā**, noklikšķiniet uz **deaktivizēt**.</span><span class="sxs-lookup"><span data-stu-id="37f20-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="37f20-108">Ziņojumu par liegtu piekļuvi var notikt arī uz koplietojamās mapes, ja vieta ir publicēšanas vietnē.</span><span class="sxs-lookup"><span data-stu-id="37f20-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="37f20-109">Informācijas, skatiet [Piekļūstot koplietojamo mapi, liegta piekļuve](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="37f20-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="37f20-110">Ja kāds saņēmu ziņojumu "Piekļuve liegta", mēģinot apskatīt piekļuves pieprasījumus, lietotāju vajadzībām pievieno kā vietu kolekcijas administratoru vai vietnes īpašnieku grupas loceklis.</span><span class="sxs-lookup"><span data-stu-id="37f20-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="37f20-111">Lai iegūtu vairāk informācijas, skatiet [Piekļuve liegta piekļuves pieprasījumu saraksts](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="37f20-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="37f20-112">Ja lietotājs saņēmu ziņojumu "Piekļuve liegta", pēc tam, kad tie tika izņemti no Active Directory uz telpām un pēc tam pievieno atpakaļ, sk. [Kad lietotāja konts ir synced Office 365 liegta piekļuve](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="37f20-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

