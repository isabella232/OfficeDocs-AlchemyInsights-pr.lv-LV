---
title: Microsoft Search fona pakalpojuma noņemšana pakalpojumā Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816203"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a><span data-ttu-id="50d5a-102">Microsoft Search fona pakalpojuma noņemšana pakalpojumā Bing</span><span class="sxs-lookup"><span data-stu-id="50d5a-102">Remove the background service for Microsoft Search in Bing</span></span>

<span data-ttu-id="50d5a-103">Lai programmā Bing noņemtu Microsoft Search fona pakalpojumu, varat izmēģināt tālāk norādītos līdzekļus.</span><span class="sxs-lookup"><span data-stu-id="50d5a-103">To remove the background service for Microsoft Search in Bing, you can try the following remedies:</span></span>

1. <span data-ttu-id="50d5a-104">Lai atgrieztos pie sākotnējā meklēšanas dzinēja iestatījumiem, rīkojieties šādi:</span><span class="sxs-lookup"><span data-stu-id="50d5a-104">To revert to the original search engine settings, do the following things:</span></span>

    <span data-ttu-id="50d5a-105">izveide.</span><span class="sxs-lookup"><span data-stu-id="50d5a-105">a.</span></span> <span data-ttu-id="50d5a-106">Pārslēdziet **opciju izmantot Bing kā noklusējuma meklēšanas [](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) programmu**.</span><span class="sxs-lookup"><span data-stu-id="50d5a-106">Switch the **Use Bing as your default search engine [toggle](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Off**.</span></span>

    <span data-ttu-id="50d5a-107">b.</span><span class="sxs-lookup"><span data-stu-id="50d5a-107">b.</span></span> <span data-ttu-id="50d5a-108">[Dodieties uz Microsoft 365 administrēšanas centru](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) un notīriet iestatījumu, kas ietekmē visus lietotājus savā organizācijā.</span><span class="sxs-lookup"><span data-stu-id="50d5a-108">[Go to the Microsoft 365 admin center](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) and clear the setting that affects all users in your organization.</span></span>

2. <span data-ttu-id="50d5a-109">Lai noņemtu fona pakalpojumu no atsevišķas ierīces, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="50d5a-109">To remove the background service from an individual device, do the following tasks:</span></span>

    <span data-ttu-id="50d5a-110">izveide.</span><span class="sxs-lookup"><span data-stu-id="50d5a-110">a.</span></span> <span data-ttu-id="50d5a-111">Izvēlieties **vadības paneļa > programmas > programmas un līdzekļi**.</span><span class="sxs-lookup"><span data-stu-id="50d5a-111">Choose **Control Panel > Programs > Programs and Features**.</span></span>

    <span data-ttu-id="50d5a-112">b.</span><span class="sxs-lookup"><span data-stu-id="50d5a-112">b.</span></span> <span data-ttu-id="50d5a-113">Instalēto programmu sarakstā ar peles labo pogu noklikšķiniet uz **Microsoft meklēšana pakalpojumā Bing** un pēc tam noklikšķiniet uz **Atinstalēt**.</span><span class="sxs-lookup"><span data-stu-id="50d5a-113">Right-click **Microsoft Search in Bing** under the list of installed programs, and then click **Uninstall**.</span></span>

3. <span data-ttu-id="50d5a-114">Lai noņemtu fona pakalpojumu no vairākām ierīcēm savā organizācijā, piesakieties kā administrators un izpildiet tālāk norādīto komandu skriptā.</span><span class="sxs-lookup"><span data-stu-id="50d5a-114">To remove the background service from multiple devices in your organization, log in as an administrator and run the following command in a script:</span></span> 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
