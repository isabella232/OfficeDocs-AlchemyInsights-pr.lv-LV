---
title: 1065 deprecation EOP izejošo IP adresi rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: f4854c32d970d84f3a0664a9e384dc6e3cd0bfa7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704604"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="a5879-102">Izslēgšanas EOP izejošo IP adrešu diapazoni</span><span class="sxs-lookup"><span data-stu-id="a5879-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="a5879-103">Mēs esam konstatējis potenciālo problēmu ar jūsu organizāciju, kas (ja nav labots līdz 26 oktobris, 2018) var pārtraukt pasta plūsmu uz jūsu lokālo vai ārējiem galamērķiem.</span><span class="sxs-lookup"><span data-stu-id="a5879-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="a5879-104">Kā iepriekš paziņots, lai vienkāršotu IP adrešu diapazona pārvaldību, mēs esam konsolidējot Exchange Online Protection (EOP) IP adrešu diapazonu, kas tiek izmantoti, lai nosūtītu un saņemtu e-pastu ārpus Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a5879-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="a5879-105">Mūsu analīze norāda, ka viens vai vairāki no ārējiem e-pasta avotiem vai galamērķiem, ko esat konfigurējis pasta plūsmas savienojumos, nepieņem savienojumus no [šeit](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)parādītā IP adrešu diapazona.</span><span class="sxs-lookup"><span data-stu-id="a5879-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="a5879-106">Act pirms oktobris 26, lai nodrošinātu, ka šie avoti un galamērķi pieņems savienojumus uz un no visām [publicētajām EOP IP adresēm](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="a5879-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="a5879-107">Lai iegūtu papildinformāciju par šīm izmaiņām, lūdzu, skatiet ziņu centra ziņas [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)vai [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="a5879-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="a5879-108">**Piezīme**: ja iepriekš izmantojāt IP vai URL publicēšana, izmantojot HTML, XML un RSS galapunkta atjauninājumus, jums ir arī migrēt uz jauno Web pakalpojumu automatizēšana šāda veida atjauninājumus.</span><span class="sxs-lookup"><span data-stu-id="a5879-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="a5879-109">Lai iegūtu papildinformāciju, skatiet [microsoft 365 galapunkta kategorijas un microsoft 365 IP adresi un URL tīmekļa pakalpojumu](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="a5879-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
