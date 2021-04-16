---
title: Veicot dubultklikšķi uz Office faila, tas netiek atvērts
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: b9c563f7dd099bf3bad9018f69e2096816dd7290
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814812"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="5246f-102">Veicot dubultklikšķi uz Office faila, tas netiek atvērts</span><span class="sxs-lookup"><span data-stu-id="5246f-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="5246f-103">Pēc dubultklikšķi uz Office faila, iespējams, redzēsit programmu atvērtu, bet pats fails netiek atvērts.</span><span class="sxs-lookup"><span data-stu-id="5246f-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="5246f-104">Vai arī var tikt parādīts šāds kļūdas ziņojums: "Nosūtot komandu programmai, radās problēma."</span><span class="sxs-lookup"><span data-stu-id="5246f-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="5246f-105">Tam ir daudz iemeslu, bet divi visbiežāk izmantotie risinājumi ir:</span><span class="sxs-lookup"><span data-stu-id="5246f-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="5246f-106">Programmā Excel pārliecinieties, vai DDE opcija ir neatzīmēta.</span><span class="sxs-lookup"><span data-stu-id="5246f-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="5246f-107">Šo opciju var atrast, izveidojot jaunu darbgrāmatu un pēc tam izvēloties Fails un **> opcijas > Papildu.**</span><span class="sxs-lookup"><span data-stu-id="5246f-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="5246f-108">Sadaļā Vispārīgi **notīriet** atzīmi no Ignorēt citas **lietojumprogrammas, kas izmanto dinamisko datu apmaiņu (Dynamic Data Exchange – DDE).**</span><span class="sxs-lookup"><span data-stu-id="5246f-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="5246f-109">Palaidiet tiešsaistes labošanu, lai atjaunotu noklusējuma iestatījumus.</span><span class="sxs-lookup"><span data-stu-id="5246f-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="5246f-110">Noklikšķiniet uz Windows pogas Sākt un meklējiet "Vadības panelis".</span><span class="sxs-lookup"><span data-stu-id="5246f-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="5246f-111">Atveriet vadības **paneli** un dodieties uz **sadaļu Programmas > programmas un līdzekļi**.</span><span class="sxs-lookup"><span data-stu-id="5246f-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="5246f-112">Pēc tam ar peles labo **pogu noklikšķiniet uz Microsoft Office [versija]** un > **labošanu tiešsaistē.**</span><span class="sxs-lookup"><span data-stu-id="5246f-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="5246f-113">Ja neviens no šiem risinājumiem [nedarbojas,](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)pilns risinājumu saraksts ir atrodams atbalsta rakstā, veicot dubultklikšķi uz Office faila, neizdodas to atvērt.</span><span class="sxs-lookup"><span data-stu-id="5246f-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
