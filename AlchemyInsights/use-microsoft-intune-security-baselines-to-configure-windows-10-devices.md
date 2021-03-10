---
title: Microsoft Intune drošības bāzes izmantošana, lai konfigurētu Windows 10 ierīces
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/10/2021
ms.locfileid: "50694435"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a><span data-ttu-id="c1708-102">Microsoft Intune drošības bāzes izmantošana Windows 10 ierīču konfigurēšanai</span><span class="sxs-lookup"><span data-stu-id="c1708-102">Use the Microsoft Intune security baselines for configuring Windows 10 devices</span></span>

<span data-ttu-id="c1708-103">Intune drošības bāzlīnijas palīdz aizsargāt lietotājus un ierīces.</span><span class="sxs-lookup"><span data-stu-id="c1708-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="c1708-104">Drošības bāzlīnijas ir Windows iestatījumi iepriekš konfigurētās grupas, ko izmanto, lai lietotu zināmo iestatījumu grupu un noklusējuma vērtības, ko iesaka atbilstošās drošības komandas.</span><span class="sxs-lookup"><span data-stu-id="c1708-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="c1708-105">Izveidojot drošības bāzes profilu pakalpojumā Intune, izveidojiet veidni, kas sastāv no vairākiem ierīces konfigurācijas profiliem.</span><span class="sxs-lookup"><span data-stu-id="c1708-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="c1708-106">Kad izvietojat drošības bāzes līnijas lietotāju vai ierīču grupām, iestatījumi tiek lietoti ierīcēs, kas darbojas operētājsistēmā Windows 10 vai jaunākās versijās.</span><span class="sxs-lookup"><span data-stu-id="c1708-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later versions.</span></span> <span data-ttu-id="c1708-107">Piemēram, automātiski izmantojot Microsoft mobilo ierīču pārvaldības (MDM) drošības bāzlīniju (1), tiek iespējots BitLocker noņemamajiem diskiem (2) ir nepieciešama parole ierīces atbloķēšanai, un (3) atspējo pamata autentifikācija.</span><span class="sxs-lookup"><span data-stu-id="c1708-107">For example, the Microsoft mobile device management (MDM) security baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="c1708-108">Ja jūsu vidē noklusējuma vērtība nedarbojas, varat pielāgot bāzes līniju, lai lietotu iestatījumus, kas nepieciešami.</span><span class="sxs-lookup"><span data-stu-id="c1708-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="c1708-109">Drošības bāzlīnijas palīdz arī izveidot end-to-end Secure Workflow pakalpojumā Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c1708-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="c1708-110">Tālāk norādītas šīs funkcionalitātes priekšrocības:</span><span class="sxs-lookup"><span data-stu-id="c1708-110">The following are some benefits of this functionality:</span></span>
- <span data-ttu-id="c1708-111">Drošības sākumdokumentā ir iekļauta paraugprakse un ieteikumi par iestatījumiem, kas ietekmē drošību.</span><span class="sxs-lookup"><span data-stu-id="c1708-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="c1708-112">Tā kā Intune partneriem ir Windows drošības grupa, kas izveido bāzes politikas bāzlīnijas, šie ieteikumi pamatojas uz stabilu orientāciju un plašu pieredzi.</span><span class="sxs-lookup"><span data-stu-id="c1708-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="c1708-113">Ja esat iesācējs darbā ar Intune un neesat pārliecināts par to, kur sākt, pēc tam drošības bāzlīnijas palīdzēs ātri izveidot un izvietot drošu profilu.</span><span class="sxs-lookup"><span data-stu-id="c1708-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="c1708-114">Ja pašlaik izmantojat grupas politiku, pēc tam migrējot uz Intune pārvaldības vajadzībām, ir daudz vienkāršāks ar drošības bāzes līnijām, jo šīs drošības bāzes ir iebūvētas Intune, kas ietver visprogresīvākās iespējas pārvaldībai.</span><span class="sxs-lookup"><span data-stu-id="c1708-114">If you are currently using a group policy, then migrating to Intune for management purposes is much easier with security baselines, because these security baselines are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="c1708-115">Papildinformāciju skatiet rakstā [Windows drošības bāzlīnijas](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) un [mobilo ierīču pārvaldība](https://docs.microsoft.com/windows/client-management/mdm/).</span><span class="sxs-lookup"><span data-stu-id="c1708-115">For more information, see [Windows security baselines](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](https://docs.microsoft.com/windows/client-management/mdm/).</span></span>