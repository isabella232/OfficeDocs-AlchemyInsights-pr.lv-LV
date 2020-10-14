---
title: Intune Win32 lietojumprogrammu izvietošana
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461872"
---
# <a name="intune-win32-app-deployment"></a><span data-ttu-id="39554-102">Intune Win32 lietojumprogrammu izvietošana</span><span class="sxs-lookup"><span data-stu-id="39554-102">Intune Win32 app deployment</span></span>

<span data-ttu-id="39554-103">Microsoft Intune atļauj Win32 lietojumprogrammas, ieskaitot, bet neaprobežojoties ar MSI. EXE ir jāizvieto Windows 10 ierīcēs.</span><span class="sxs-lookup"><span data-stu-id="39554-103">Microsoft Intune allows Win32 applications, including but not limited to MSI and .EXE’s to be deployed to Windows 10 devices.</span></span> <span data-ttu-id="39554-104">Izmantotajam izvietošanas mehānismam ir nepieciešams, lai Intune pārvaldības paplašinājums (IME) būtu atrodams Target ierīcē.</span><span class="sxs-lookup"><span data-stu-id="39554-104">The deployment mechanism used requires the Intune Management Extension (IME) to be present on the target device.</span></span> <span data-ttu-id="39554-105">Pēc PowerShell skripta vai Win32 lietojumprogrammas izvietošanas uz lietotāju/ierīci tiek automātiski instalēts IME.</span><span class="sxs-lookup"><span data-stu-id="39554-105">The IME will be installed automatically as a result of targeting a powershell script or win32 application deployment to a user / device.</span></span>

<span data-ttu-id="39554-106">Pastāv arī priekšnosacījumu kopa, kas ir jāizpilda, lai izvietotu Win32 lietojumprogrammas, kas ietver:</span><span class="sxs-lookup"><span data-stu-id="39554-106">There are also a set of pre-requisites which must be met in order to deploy Win32 apps which include:</span></span>

- <span data-ttu-id="39554-107">Atbalstītās platformas: Windows 10 versija 1607 vai jaunāka (Enterprise, Pro un Education versijas).</span><span class="sxs-lookup"><span data-stu-id="39554-107">Supported platforms: Windows 10 version 1607 or later (Enterprise, Pro, and Education versions).</span></span>
- <span data-ttu-id="39554-108">Atbalstītā arhitektūra: x86 un x64.</span><span class="sxs-lookup"><span data-stu-id="39554-108">Supported architecture: x86 and x64.</span></span>
- <span data-ttu-id="39554-109">Ierīču pārvaldība: AAD ir pievienojies un automātiski reģistrējušies (ieskaitot hibrīdo domēnu un grupas politiku, kas tiek automātiski reģistrēta).</span><span class="sxs-lookup"><span data-stu-id="39554-109">Device Management: AAD joined and auto-enrolled (including hybrid domain joined and group policy auto-enrolled).</span></span>
- <span data-ttu-id="39554-110">Lietojumprogrammas pakotnes formāts: **intunewin**  failu, ko sagatavojis [Microsoft Win32 satura sagatavošanas rīks](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span><span class="sxs-lookup"><span data-stu-id="39554-110">Application Package format: .**intunewin**  file prepared by the [Microsoft Win32 content Prep tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span></span>
- <span data-ttu-id="39554-111">Ierobežojumi</span><span class="sxs-lookup"><span data-stu-id="39554-111">Limitations:</span></span>
    - <span data-ttu-id="39554-112">Maksimālais lielums: 8GB.</span><span class="sxs-lookup"><span data-stu-id="39554-112">Maximum size: 8GB.</span></span>
    - <span data-ttu-id="39554-113">Neatbalstītā arhitektūra: ieroči.</span><span class="sxs-lookup"><span data-stu-id="39554-113">Unsupported architecture: ARMs.</span></span>

<span data-ttu-id="39554-114">Lai skatītu informāciju, kas saistīta ar šīm darbībām, recenzējiet dokumentu "[pievienot, piešķirt un pārraudzīt Win32 lietojumprogrammu pakalpojumā Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)".</span><span class="sxs-lookup"><span data-stu-id="39554-114">Review the doc "[Add, assign, and monitor a Win32 app in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" for information related to those steps.</span></span>

<span data-ttu-id="39554-115">Detalizētu informāciju par problēmu novēršanu lietojumprogrammas izvietojumā sistēmā Windows, tostarp Win32 lietojumprogrammas, var pārskatīt šādos dokumentos</span><span class="sxs-lookup"><span data-stu-id="39554-115">Details on troubleshooting application deployment on Windows including Win32 apps can be reviewed in the following documents</span></span>

- [<span data-ttu-id="39554-116">Lietojumprogrammas instalēšanas problēmu novēršana</span><span class="sxs-lookup"><span data-stu-id="39554-116">Troubleshoot App Installation issues</span></span>](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [<span data-ttu-id="39554-117">Win32 lietojumprogrammu problēmu novēršana</span><span class="sxs-lookup"><span data-stu-id="39554-117">Troubleshoot Win32 Apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)