---
title: Datu atrašanās vieta
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: 0e683c8266d425be95e87c590d4cb5d56108721a
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207268"
---
# <a name="data-location"></a><span data-ttu-id="ebb79-102">Datu atrašanās vieta</span><span class="sxs-lookup"><span data-stu-id="ebb79-102">Data location</span></span>

<span data-ttu-id="ebb79-103">Varat skatīt Office 365 nomnieka atrašanās vietu administrēšanas centrā vai, izveidojot savienojumu ar Exchange Online, izmantojot PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ebb79-103">You can view the location of your Office 365 tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="ebb79-104">**Administrēšanas centrs:**</span><span class="sxs-lookup"><span data-stu-id="ebb79-104">**Admin center:**</span></span>
1. <span data-ttu-id="ebb79-105">Piesakieties [administrēšanas centrā](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="ebb79-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="ebb79-106">Atlasiet vienumu **Iestatījumi** > **organizācijas profils**.</span><span class="sxs-lookup"><span data-stu-id="ebb79-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="ebb79-107">Sadaļā **datu atrašanās vieta**atlasiet **Skatīt detalizētu informāciju**.</span><span class="sxs-lookup"><span data-stu-id="ebb79-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="ebb79-108">**Powershell:**</span><span class="sxs-lookup"><span data-stu-id="ebb79-108">**PowerShell:**</span></span>
1. <span data-ttu-id="ebb79-109">Izveidot savienojumu ar Exchange Online, izmantojot programmu Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ebb79-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="ebb79-110">Izpildīt [Get OrganizationalUnit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet, lai parādītu sarakstu ar nomnieka rekvizītus.</span><span class="sxs-lookup"><span data-stu-id="ebb79-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant’s properties.</span></span> 
3. <span data-ttu-id="ebb79-111">Apskatiet rekvizītu OrganizationId.</span><span class="sxs-lookup"><span data-stu-id="ebb79-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="ebb79-112">Ja jums ir EXO un SPO datu atrašanās vieta, varat noteikt datu atrašanās vietu citiem pakalpojumiem, kurus jūs varat izmantot no vietas, [kur atrodas jūsu dati](https://products.office.com/where-is-your-data-located).</span><span class="sxs-lookup"><span data-stu-id="ebb79-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>