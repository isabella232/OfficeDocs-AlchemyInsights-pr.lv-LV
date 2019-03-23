---
title: 1065 EOP izslēgšanas izejošo IP adresi rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 0def0a93c61ea762918f1c9e6edb2e9b04446851
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/22/2019
ms.locfileid: "30777278"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="5e658-102">EOP izejošo IP adresi diapazoni izslēgšanas</span><span class="sxs-lookup"><span data-stu-id="5e658-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="5e658-103">Mēs esam atklāti potenciālu problēmu ar savu organizāciju, kas (ja netiek laboti ar oktobrī 26, 2018) nepārtrūks pasta plūsma uz lokālajiem vai ārējiem mērķiem.</span><span class="sxs-lookup"><span data-stu-id="5e658-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="5e658-104">Kā iepriekš paziņota, vienkāršot IP adrešu diapazona vadību, mēs konsolidēšana Exchange Online aizsardzība (EOP) IP adrese diapazonus, ko izmanto, lai nosūtītu un saņemtu e-pastu ārpus biroja 365.</span><span class="sxs-lookup"><span data-stu-id="5e658-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365.</span></span> <span data-ttu-id="5e658-105">Mūsu analīze liecina, ka vienai vai vairākām no ārējiem e-pasta avotu vai galamērķiem, pasta plūsmas savienotāji konfigurētajā nav akceptēt savienojumus no IP adrešu diapazonu parādīts [šeit](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="5e658-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="5e658-106">Darboties pirms oktobris 26, lai nodrošinātu šos avotus un galamērķiem tiks akceptēšanai un no visiem [publicēts EOP IP adreses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="5e658-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="5e658-107">Plašāku informāciju par šo izmaiņu, lūdzu, skatiet ziņojumu centra amatu, [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)vai [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="5e658-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>
  
 <span data-ttu-id="5e658-108">**Piezīme**: ja iepriekš izmantojāt IP vai URL publicēšana, izmantojot HTML, XML un RSS galapunkta atjauninājumus, jums arī vajadzētu pāriet uz jaunajos web pakalpojumos, automatizējot šo atjauninājumu tipiem.</span><span class="sxs-lookup"><span data-stu-id="5e658-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="5e658-109">Lai iegūtu papildinformāciju, skatiet [Office 365 IP adrese un biroja 365 galapunkta kategorijām un URL web pakalpojums](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="5e658-109">For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
  

