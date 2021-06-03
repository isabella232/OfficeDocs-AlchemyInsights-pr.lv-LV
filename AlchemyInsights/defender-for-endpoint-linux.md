---
title: Microsoft Defender galapunktam operētājsistēmā Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11490"
- "9001464"
ms.openlocfilehash: 99894d83c51e11ea6dd1746568762eac856306b3
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731675"
---
# <a name="microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="3158d-102">Microsoft Defender galapunktam operētājsistēmā Linux</span><span class="sxs-lookup"><span data-stu-id="3158d-102">Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="3158d-103">Detalizētu Linux dokumentāciju skatiet rakstā [Microsoft Defender galapunktam operētājsistēmā Linux.](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux)</span><span class="sxs-lookup"><span data-stu-id="3158d-103">For detailed Linux documentation, see [Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux).</span></span>

<span data-ttu-id="3158d-104">Informāciju par sistēmu un instalāciju skatiet rakstā:</span><span class="sxs-lookup"><span data-stu-id="3158d-104">For system and installation information, see:</span></span>

- [<span data-ttu-id="3158d-105">Priekšnosacījumi</span><span class="sxs-lookup"><span data-stu-id="3158d-105">Prerequisites</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#prerequisites)
- [<span data-ttu-id="3158d-106">Sistēmas prasības</span><span class="sxs-lookup"><span data-stu-id="3158d-106">System requirements</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#system-requirements)
- [<span data-ttu-id="3158d-107">Instalēšanas norādījumi</span><span class="sxs-lookup"><span data-stu-id="3158d-107">Installation instructions</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#installation-instructions)
- [<span data-ttu-id="3158d-108">Tīkla savienojumi</span><span class="sxs-lookup"><span data-stu-id="3158d-108">Network connections</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#network-connections)

<span data-ttu-id="3158d-109">Norādījumus skatiet tālāk redzamajā sadaļā.</span><span class="sxs-lookup"><span data-stu-id="3158d-109">For instructions, see:</span></span>

- [<span data-ttu-id="3158d-110">Ierīces starpniekservera un interneta savienojuma iestatījumu konfigurēšana</span><span class="sxs-lookup"><span data-stu-id="3158d-110">Configure device proxy and Internet connectivity settings</span></span>](/microsoft-365/security/defender-endpoint/configure-proxy-internet#enable-access-to-microsoft-defender-atp-service-urls-in-the-proxy-server)
- [<span data-ttu-id="3158d-111">Microsoft Defender galapunkta atjauninājumu izvietošana operētājsistēmā Linux</span><span class="sxs-lookup"><span data-stu-id="3158d-111">Deploy updates for Microsoft Defender for Endpoint on Linux</span></span>](/microsoft-365/security/defender-endpoint/linux-updates)
- [<span data-ttu-id="3158d-112">Kā operētājsistēmā Linux konfigurēt Microsoft Defender galapunktam</span><span class="sxs-lookup"><span data-stu-id="3158d-112">How to configure Microsoft Defender for Endpoint on Linux</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#how-to-configure-microsoft-defender-for-endpoint-on-linux)
- [<span data-ttu-id="3158d-113">Atbalstītās komandas</span><span class="sxs-lookup"><span data-stu-id="3158d-113">Supported commands</span></span>](/microsoft-365/security/defender-endpoint/linux-resources#supported-commands)

## <a name="i-need-help"></a><span data-ttu-id="3158d-114">Man nepieciešama palīdzība!</span><span class="sxs-lookup"><span data-stu-id="3158d-114">I need help!</span></span>

<span data-ttu-id="3158d-115">Ja nevarat atrast meklēto informāciju/palīdzību, precizējiet meklēšanas virkni.</span><span class="sxs-lookup"><span data-stu-id="3158d-115">If you can't find the information/help you're looking for, refine your search string.</span></span>

<span data-ttu-id="3158d-116">Pirms sazināties ar Microsoft atbalsta dienestu, noteikti apkopojiet jūsu problēmas izpētei nepieciešamos datus un pievienojiet tos biļetei.</span><span class="sxs-lookup"><span data-stu-id="3158d-116">Before contacting Microsoft Support, make sure to collect the data required to investigate your issue, and attach it to the ticket.</span></span> <span data-ttu-id="3158d-117">Lai uzzinātu, kā apkopot diagnostikas informāciju, skatiet sadaļu [Diagnostikas datu apkopošana.](/microsoft-365/security/defender-endpoint/linux-resources#collect-diagnostic-information)</span><span class="sxs-lookup"><span data-stu-id="3158d-117">For steps to collect the diagnosic information, see [Collect diagnostic data](/microsoft-365/security/defender-endpoint/linux-resources#collect-diagnostic-information).</span></span>