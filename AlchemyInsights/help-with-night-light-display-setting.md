---
title: Palīdzība par nakts gaismas displeja iestatījumu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404665"
---
# <a name="help-with-the-night-light-display-setting"></a><span data-ttu-id="fc591-102">Palīdzība par nakts gaismas displeja iestatījumu</span><span class="sxs-lookup"><span data-stu-id="fc591-102">Help with the night light display setting</span></span>

<span data-ttu-id="fc591-103">Papildinformāciju par nakts laika displeja iestatījumiem skatiet [rakstā Displeja iestatīšana nakts laikam operētājsistēmā Windows 10.](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)</span><span class="sxs-lookup"><span data-stu-id="fc591-103">To learn more about night time display settings, see [Set your display for night time in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span></span>

<span data-ttu-id="fc591-104">Ja nakts gaismas opcijas iestatījumos ir pelēkotas, skatiet displeja draiveri:</span><span class="sxs-lookup"><span data-stu-id="fc591-104">If the night light options are grayed out in Settings, check your display driver:</span></span> 

1. <span data-ttu-id="fc591-105">Uzdevumjoslā noklikšķiniet uz meklēšanas lodziņa **un ierakstiet Ierīču** pārvaldnieks un pēc tam meklēšanas **rezultātos** atlasiet Ierīču pārvaldnieks.</span><span class="sxs-lookup"><span data-stu-id="fc591-105">Click the search box on your taskbar and type **Device Manager**, and then select **Device Manager** in the search results.</span></span>
1. <span data-ttu-id="fc591-106">Izvērsiet **displeja adapterus**.</span><span class="sxs-lookup"><span data-stu-id="fc591-106">Expand **Display adapters**.</span></span> 

<span data-ttu-id="fc591-107">Diemžēl nakts gaismas līdzeklis nav pieejams, ja jūsu ierīce izmanto DisplayLink draiveri vai pamata displeja draiveri.</span><span class="sxs-lookup"><span data-stu-id="fc591-107">Unfortunately, the night light feature is not available if your device uses a DisplayLink driver or a Basic Display driver.</span></span>

<span data-ttu-id="fc591-108">Nakts gaismas līdzeklis izmanto jaunākās grafikas tehnoloģijas, tāpēc, iespējams, būs jāatjaunina displeja draiveris:</span><span class="sxs-lookup"><span data-stu-id="fc591-108">The night light feature makes use of recent graphics technology, so you might need to update your display driver:</span></span>  

- <span data-ttu-id="fc591-109">Pārbaudiet, vai nav atjauninājumu, **dodoties uz Sākums**  >  **Iestatījumu**  >  **atjaunināšanas &** Windows  >  **Update**  >  **pārbaudīt, vai nav atjauninājumu.**</span><span class="sxs-lookup"><span data-stu-id="fc591-109">Check for updates by going to **Start** > **Settings** > **Update & Security** > **Windows Update** > **Check for Updates**.</span></span>  

<span data-ttu-id="fc591-110">VAI</span><span class="sxs-lookup"><span data-stu-id="fc591-110">OR</span></span>

- <span data-ttu-id="fc591-111">Apmeklējiet aparatūras ražotāja atbalsta tīmekļa vietni, lai manuāli lejupielādētu un instalētu jaunākos displeja draiverus.</span><span class="sxs-lookup"><span data-stu-id="fc591-111">Visit your hardware manufacturer's support website to manually download and install the latest display drivers.</span></span>

## <a name="reset-night-light-in-the-registry"></a><span data-ttu-id="fc591-112">Atiestatīt nakts gaismu reģistrā</span><span class="sxs-lookup"><span data-stu-id="fc591-112">Reset night light in the registry</span></span>

<span data-ttu-id="fc591-113">Ja displeja draivera atjaunināšana nedarbojas, iespējams, būs jāatiestata nakts gaisma reģistrā.</span><span class="sxs-lookup"><span data-stu-id="fc591-113">If updating your display driver didn't work, you might need to reset night light in the registry.</span></span>  

<span data-ttu-id="fc591-114">**Uzmanību!** Šī problēmu novēršanas darbība ir ieteicama tikai pieredzējušiem lietotājiem.</span><span class="sxs-lookup"><span data-stu-id="fc591-114">**Caution:** This troubleshooting step is recommended only for advanced users.</span></span> <span data-ttu-id="fc591-115">Nepareizi modificējot reģistru, iespējamas nopietnas problēmas.</span><span class="sxs-lookup"><span data-stu-id="fc591-115">Serious problems can occur if you modify the registry incorrectly.</span></span> <span data-ttu-id="fc591-116">Lai nodrošinātu papildu aizsardzību, dublējiet reģistru, pirms to modificējat, lai varētu to atjaunot, ja rodas problēmas.</span><span class="sxs-lookup"><span data-stu-id="fc591-116">For added protection, back up the registry before you modify it so  you can restore it if problems occur.</span></span>

1. <span data-ttu-id="fc591-117">Meklēšanas lodziņā ierakstiet **regedit un** pēc tam meklēšanas **rezultātos atlasiet** Reģistra redaktors.</span><span class="sxs-lookup"><span data-stu-id="fc591-117">In the search box, type **regedit**, and then select **Registry Editor** in the search results.</span></span>

1. <span data-ttu-id="fc591-118">Dodieties uz šo reģistra atslēgu:</span><span class="sxs-lookup"><span data-stu-id="fc591-118">Go to the following registry key:</span></span> 

    <span data-ttu-id="fc591-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span><span class="sxs-lookup"><span data-stu-id="fc591-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span></span>

1. <span data-ttu-id="fc591-120">Eksportējiet un pēc tam izdzēsiet šo apakšatslēgu:$$windows.data.bluelightreduction.bluelightreductionstate</span><span class="sxs-lookup"><span data-stu-id="fc591-120">Export and then delete the following subkey:$$windows.data.bluelightreduction.bluelightreductionstate</span></span>

1. <span data-ttu-id="fc591-121">Eksportējiet un pēc tam izdzēsiet šo apakšatslēgu:$$windows.data.bluelightreduction.settings</span><span class="sxs-lookup"><span data-stu-id="fc591-121">Export and then delete the following subkey:$$windows.data.bluelightreduction.settings</span></span>

1. <span data-ttu-id="fc591-122">Restartējiet Windows un pārbaudiet, vai ir pieejamas nakts gaismas opcijas.</span><span class="sxs-lookup"><span data-stu-id="fc591-122">Restart Windows and verify if the night light options are available.</span></span>


