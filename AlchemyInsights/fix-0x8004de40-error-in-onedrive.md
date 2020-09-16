---
title: 0x8004de40 kļūdas novēršana pakalpojumā OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745137"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="296a2-102">0x8004de40 kļūdas novēršana pakalpojumā OneDrive</span><span class="sxs-lookup"><span data-stu-id="296a2-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="296a2-103">Ja saņemat 0x8004de40 kļūdu pakalpojumā OneDrive:</span><span class="sxs-lookup"><span data-stu-id="296a2-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="296a2-104">Atsāknējiet ietekmēto datoru, kamēr ir izveidots savienojums ar savu aktivs direktorija domēnu.</span><span class="sxs-lookup"><span data-stu-id="296a2-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="296a2-105">Ja atsāknēšana nenovērš problēmu, Atsaistiet un atkārtoti Pievienojieties ierīcei no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="296a2-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="296a2-106">**Piezīme**. veicot šīs darbības, jums jāatrodas korporatīvajā tīklā.</span><span class="sxs-lookup"><span data-stu-id="296a2-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="296a2-107">Neveiciet šīs darbības, ja nevarat izveidot savienojumu ar savas korporatīvās infrastruktūras (piemēram, ceļojuma laikā).</span><span class="sxs-lookup"><span data-stu-id="296a2-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="296a2-108">Atveriet privileģētu komandu uzvedni.</span><span class="sxs-lookup"><span data-stu-id="296a2-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="296a2-109">Lai atvērtu privileģētu komandu uzvedni, noklikšķiniet uz **Sākt**, ar peles labo pogu noklikšķiniet uz **komandu uzvedne**un pēc tam noklikšķiniet uz **Palaist kā administratoram**.</span><span class="sxs-lookup"><span data-stu-id="296a2-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="296a2-110">Ierakstiet *dsregcmd/Leave* un nospiediet taustiņu **Enter**.</span><span class="sxs-lookup"><span data-stu-id="296a2-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="296a2-111">Kad tas ir paveikts, ierakstiet *dsregcmd/Join* un nospiediet taustiņu **Enter**.</span><span class="sxs-lookup"><span data-stu-id="296a2-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="296a2-112">Kad tas ir paveikts, izvērsiet komandu uzvedni.</span><span class="sxs-lookup"><span data-stu-id="296a2-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="296a2-113">Restartējiet datoru un piesakieties pakalpojumā OneDrive.</span><span class="sxs-lookup"><span data-stu-id="296a2-113">Reboot the computer, and log into OneDrive.</span></span>