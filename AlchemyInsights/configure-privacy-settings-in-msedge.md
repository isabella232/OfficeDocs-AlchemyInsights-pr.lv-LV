---
title: Konfidencialitātes iestatījumu konfigurēšana programmā Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 2367a7a55d1837fa7c7095fd0ac10ff1cf7ae72d
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405104"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a><span data-ttu-id="eb7af-102">Konfidencialitātes iestatījumu konfigurēšana programmā Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="eb7af-102">Configure privacy settings in Microsoft Edge</span></span>

<span data-ttu-id="eb7af-103">Pēc noklusējuma, ja microsoft Edge ir izvietots platformās, kas nav Windows platformas, diagnostikas dati un vietņu informācija netiek nosūtīti korporācijai Microsoft.</span><span class="sxs-lookup"><span data-stu-id="eb7af-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information aren't sent to Microsoft.</span></span> <span data-ttu-id="eb7af-104">Tomēr, ja operētājsistēmā Windows 10 ir izvietota programmatūra Microsoft Edge, diagnostikas dati un vietnes informācija tiek sūtīta atbilstoši [lietotāja Windows diagnostikas datu iestatījumiem.](https://go.microsoft.com/fwlink/?linkid=2132472)</span><span class="sxs-lookup"><span data-stu-id="eb7af-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://go.microsoft.com/fwlink/?linkid=2132472).</span></span>

<span data-ttu-id="eb7af-105">Lai konfigurētu, kā Microsoft Edge apstrādā datu apkopošanu jūsu organizācijā, izmantojiet šādas grupas politikas:</span><span class="sxs-lookup"><span data-stu-id="eb7af-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="eb7af-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) ieslēdz ziņošanu par lietojumu un ar avāriju saistītiem datiem.</span><span class="sxs-lookup"><span data-stu-id="eb7af-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) turns on reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="eb7af-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) nosūta vietnes informāciju, kas tiek izmantota Microsoft pakalpojumu uzlabošanai.</span><span class="sxs-lookup"><span data-stu-id="eb7af-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) sends site information used to improve Microsoft services.</span></span>

<span data-ttu-id="eb7af-108">Papildinformāciju skatiet rakstā [Politikas iestatījumu konfigurēšana.](https://go.microsoft.com/fwlink/?linkid=2132577)</span><span class="sxs-lookup"><span data-stu-id="eb7af-108">To learn more, see [Configure policy settings](https://go.microsoft.com/fwlink/?linkid=2132577).</span></span>
