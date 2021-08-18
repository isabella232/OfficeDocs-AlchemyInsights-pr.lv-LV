---
title: Microsoft Edge iestatījumu konfigurēšana
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
ms.openlocfilehash: 24721325aefd4a8c0dbeb7864ce6da637c4df932694d4b6fff80cab5bb5b4319
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114179"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge iestatījumu konfigurēšana

Pēc noklusējuma, Microsoft Edge ir izvietotas platformās, kas nav Windows platformas, diagnostikas dati un vietnes informācija netiek sūtīta korporācijai Microsoft. Tomēr, ja Microsoft Edge vai Windows 10, diagnostikas dati un vietnes informācija tiek sūtīta saskaņā ar lietotāju [Windows diagnostikas datu iestatījumiem.](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)

Lai konfigurētu Microsoft Edge datu apkopošanu jūsu organizācijai, izmantojiet šādas grupas politikas:
- [MetricsReportingEnabled: šī](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled)politika ļauj ziņot par lietojumu un ar avāriju saistītiem datiem.
- [SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): Šī politika nosūta vietnes informāciju, kas tiek izmantota, lai uzlabotu Microsoft pakalpojumi.

Papildinformāciju skatiet rakstā [Politikas iestatījumu konfigurēšana.](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings)