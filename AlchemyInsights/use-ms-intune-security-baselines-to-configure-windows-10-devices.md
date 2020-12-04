---
title: Microsoft Intune drošības bāzes izmantošana, lai konfigurētu Windows 10 ierīces
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573538"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="0c4d8-102">Microsoft Intune drošības bāzes izmantošana, lai konfigurētu Windows 10 ierīces</span><span class="sxs-lookup"><span data-stu-id="0c4d8-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="0c4d8-103">Intune drošības bāzlīnijas palīdz aizsargāt lietotājus un ierīces.</span><span class="sxs-lookup"><span data-stu-id="0c4d8-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="0c4d8-104">Drošības bāzlīnijas ir Windows iestatījumi iepriekš konfigurētās grupas, ko izmanto, lai lietotu zināmo iestatījumu grupu un noklusējuma vērtības, ko iesaka atbilstošās drošības komandas.</span><span class="sxs-lookup"><span data-stu-id="0c4d8-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="0c4d8-105">Izveidojot drošības bāzes profilu pakalpojumā Intune, izveidojiet veidni, kas sastāv no vairākiem ierīces konfigurācijas profiliem.</span><span class="sxs-lookup"><span data-stu-id="0c4d8-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="0c4d8-106">Kad izvietojat drošības bāzes līnijas lietotāju vai ierīču grupām, iestatījumi tiek lietoti ierīcēs, kas darbojas operētājsistēmā Windows 10 vai jaunākā versijā.</span><span class="sxs-lookup"><span data-stu-id="0c4d8-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="0c4d8-107">Piemēram, MDM drošības bāzlīnija automātiski (1) iespējo BitLocker noņemamiem diskiem (2), ir nepieciešama parole ierīces bloķēšanai, un (3) atspējo pamata autentifikāciju.</span><span class="sxs-lookup"><span data-stu-id="0c4d8-107">For example, MDM Security Baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="0c4d8-108">Ja jūsu vidē noklusējuma vērtība nedarbojas, pielāgojiet bāzes līniju, lai lietotu iestatījumus, kas nepieciešami.</span><span class="sxs-lookup"><span data-stu-id="0c4d8-108">When a default value doesn't work for your environment, customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="0c4d8-109">Drošības bāzlīnijas palīdz arī izveidot end-to-end Secure Workflow pakalpojumā Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0c4d8-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="0c4d8-110">Tālāk ir norādītas dažas priekšrocības:</span><span class="sxs-lookup"><span data-stu-id="0c4d8-110">The following are some benefits of this:</span></span>

- <span data-ttu-id="0c4d8-111">Drošības sākumdokumentā ir iekļauta paraugprakse un ieteikumi par iestatījumiem, kas ietekmē drošību.</span><span class="sxs-lookup"><span data-stu-id="0c4d8-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="0c4d8-112">Tā kā Intune partneriem ir Windows drošības grupa, kas izveido bāzes politikas bāzlīnijas, šie ieteikumi pamatojas uz stabilu orientāciju un plašu pieredzi.</span><span class="sxs-lookup"><span data-stu-id="0c4d8-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="0c4d8-113">Ja esat iesācējs darbā ar Intune un neesat pārliecināts par to, kur sākt, pēc tam drošības bāzlīnijas palīdzēs ātri izveidot un izvietot drošu profilu.</span><span class="sxs-lookup"><span data-stu-id="0c4d8-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="0c4d8-114">Ja pašlaik izmantojat grupas politiku, pēc tam migrēšana uz Intune pārvaldības vajadzībām ir daudz vienkāršāka ar drošības bāzes līnijām, jo tās ir iebūvētas Intune un ietver visprogresīvākās iespējas pārvaldībai.</span><span class="sxs-lookup"><span data-stu-id="0c4d8-114">If you currently use a group policy, then migrating to Intune for management purposes is much easier with security baselines, because they are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="0c4d8-115">Papildinformāciju skatiet rakstā [Windows drošības bāzlīnijas](https://go.microsoft.com/fwlink/?linkid=2141503) un [mobilo ierīču pārvaldība](https://go.microsoft.com/fwlink/?linkid=2141701).</span><span class="sxs-lookup"><span data-stu-id="0c4d8-115">To learn more, see [Windows security baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile device management](https://go.microsoft.com/fwlink/?linkid=2141701).</span></span>