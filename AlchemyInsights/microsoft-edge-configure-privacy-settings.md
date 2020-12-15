---
title: Microsoft Edge konfidencialitātes iestatījumu konfigurēšana
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: dcd1d91dcde1f585caf0e1e3af30946513a0f26c
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677795"
---
# <a name="microsoft-edge-configure-privacy-settings"></a><span data-ttu-id="80b5a-102">Microsoft Edge konfidencialitātes iestatījumu konfigurēšana</span><span class="sxs-lookup"><span data-stu-id="80b5a-102">Microsoft Edge configure privacy settings</span></span>

<span data-ttu-id="80b5a-103">Pēc noklusējuma, ja Microsoft Edge ir izvietots platformā non-Windows, diagnostikas dati un vietnes informācija netiek nosūtīta korporācijai Microsoft.</span><span class="sxs-lookup"><span data-stu-id="80b5a-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information are not sent to Microsoft.</span></span> <span data-ttu-id="80b5a-104">Tomēr, ja Microsoft Edge ir izvietots operētājsistēmā Windows 10, diagnostikas dati un vietnes informācija tiek nosūtīta atbilstoši lietotāju [Windows diagnostikas datu iestatījumiem](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span><span class="sxs-lookup"><span data-stu-id="80b5a-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span></span>

<span data-ttu-id="80b5a-105">Lai konfigurētu, kā Microsoft Edge apstrādā datu apkopošanu savai organizācijai, izmantojiet tālāk norādītās grupu politikas.</span><span class="sxs-lookup"><span data-stu-id="80b5a-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="80b5a-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): šī politika sniedz atskaišu izveides un ar avarēšanu saistītus datus.</span><span class="sxs-lookup"><span data-stu-id="80b5a-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): This policy enables reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="80b5a-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): šī politika nosūta vietnes informāciju, kas tiek izmantota, lai uzlabotu Microsoft pakalpojumus.</span><span class="sxs-lookup"><span data-stu-id="80b5a-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): This policy sends site information that is used to improve Microsoft services.</span></span>

<span data-ttu-id="80b5a-108">Papildinformāciju skatiet rakstā [politikas iestatījumu konfigurēšana](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span><span class="sxs-lookup"><span data-stu-id="80b5a-108">To learn more, see [Configure policy settings](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span></span>