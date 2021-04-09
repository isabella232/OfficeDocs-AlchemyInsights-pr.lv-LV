---
title: Pakalpojuma 0x8004de40 labošana pakalpojumā OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649755"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="db858-102">Pakalpojuma 0x8004de40 labošana pakalpojumā OneDrive</span><span class="sxs-lookup"><span data-stu-id="db858-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="db858-103">Ja jūsu datorā darbojas sistēma Windows 7 un tiek parādīta šī kļūda, atjauniniet, lai iespējotu [TLS 1.1 un TLS 1.2 kā noklusējuma drošos protokolus sistēmā WinHTTP sistēmā Windows.](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)</span><span class="sxs-lookup"><span data-stu-id="db858-103">If you're running Windows 7 and receive this error, [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

<span data-ttu-id="db858-104">Ja datorā darbojas operētājsistēma Windows 10 un saņemat kļūdas 0x8004de40 saistībā ar OneDrive:</span><span class="sxs-lookup"><span data-stu-id="db858-104">If you're running Windows 10, and you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="db858-105">Restartējiet ietekmēto datoru, kamēr ir izveidots savienojums ar pakalpojuma Acitve direktorija domēnu.</span><span class="sxs-lookup"><span data-stu-id="db858-105">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="db858-106">Ja atkārtota palaišana nenovērš problēmu, atkārtoti pievienojiet ierīci no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="db858-106">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="db858-107">**Piezīme.** Jums ir jābūt korporatīvajā tīklā, veicot šīs darbības.</span><span class="sxs-lookup"><span data-stu-id="db858-107">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="db858-108">Neveiciet šīs darbības, ja neesat izveidojis savienojumu ar savu korporatīvo infrastruktūru (piemēram, atrodoties braucot).</span><span class="sxs-lookup"><span data-stu-id="db858-108">Don't perform these steps when you aren't connected to your corporate infrastructure (for example, while traveling).</span></span> 

1. <span data-ttu-id="db858-109">Atveriet priviliģētu komandu uzvedni, atlasot **Sākums**, ar peles labo **pogu** noklikšķiniet uz Komandu uzvedne un pēc tam atlasiet Palaist **kā administratoram.**</span><span class="sxs-lookup"><span data-stu-id="db858-109">Open an elevated command prompt by selecting **Start**, right-click **Command Prompt**, and then select **Run as administrator**.</span></span>

1. <span data-ttu-id="db858-110">Ierakstiet *dsregcmd /leave un* nospiediet taustiņu **Enter.**</span><span class="sxs-lookup"><span data-stu-id="db858-110">Type *dsregcmd /leave* and press **Enter**.</span></span>

1. <span data-ttu-id="db858-111">Kad tas ir pabeigts, *ierakstiet dsregcmd /join un* nospiediet taustiņu **Enter.**</span><span class="sxs-lookup"><span data-stu-id="db858-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>

1. <span data-ttu-id="db858-112">Kad esat pabeidzis, aizveriet komandu uzvedni.</span><span class="sxs-lookup"><span data-stu-id="db858-112">When complete, close the command prompt.</span></span>

1. <span data-ttu-id="db858-113">Restartējiet datoru un piesakieties pakalpojumā OneDrive.</span><span class="sxs-lookup"><span data-stu-id="db858-113">Reboot the computer, and log into OneDrive.</span></span>