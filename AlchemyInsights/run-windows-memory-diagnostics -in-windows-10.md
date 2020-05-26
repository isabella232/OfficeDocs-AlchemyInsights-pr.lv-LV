---
title: Windows atmiņas diagnostikas palaišana operētājsistēmā Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/19/2020
ms.locfileid: "44357789"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="5cf44-102">Windows atmiņas diagnostikas palaišana operētājsistēmā Windows 10</span><span class="sxs-lookup"><span data-stu-id="5cf44-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="5cf44-103">Ja Windows un lietojumprogrammas datorā avarē, sasalst vai darbojas nestabilā veidā, var rasties problēmas ar datora atmiņu (RAM).</span><span class="sxs-lookup"><span data-stu-id="5cf44-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="5cf44-104">Windows atmiņas diagnostiku var palaist, lai meklētu problēmas ar datora RAM.</span><span class="sxs-lookup"><span data-stu-id="5cf44-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="5cf44-105">Uzdevumjoslas meklēšanas lodziņā ierakstiet **atmiņas diagnostika**un pēc tam atlasiet **Windows atmiņas diagnostika**.</span><span class="sxs-lookup"><span data-stu-id="5cf44-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="5cf44-106">Lai palaistu diagnostiku, DATORAM ir jārestartē.</span><span class="sxs-lookup"><span data-stu-id="5cf44-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="5cf44-107">Jums ir iespēja nekavējoties restartēt (Lūdzu, saglabājiet savu darbu un aizveriet atvērtos dokumentus un e-pasta ziņojumus vispirms) vai ieplānojiet diagnostiku, lai tas tiktu palaists automātiski nākamajā datora restartēšanas reizē.</span><span class="sxs-lookup"><span data-stu-id="5cf44-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Windows atmiņas diagnostika](media/windows-memory-diagnostic.png)

<span data-ttu-id="5cf44-109">Kad dators tiek restartēts, **Windows atmiņas diagnostikas rīks** darbosies automātiski.</span><span class="sxs-lookup"><span data-stu-id="5cf44-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="5cf44-110">Status un progress tiks parādīts kā diagnostika palaist, un jums ir iespēja atcelt diagnostiku, hitting **ESC** taustiņu uz klaviatūras.</span><span class="sxs-lookup"><span data-stu-id="5cf44-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="5cf44-111">Kad diagnostika ir pabeigta, sistēma Windows tiks startēta kā parasti.</span><span class="sxs-lookup"><span data-stu-id="5cf44-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="5cf44-112">Uzreiz pēc restartēšanas, kad tiek parādīta darbvirsma, tiek parādīts paziņojums (blakus **darbību centra** ikonai uzdevumjoslā), lai norādītu, vai ir atrastas atmiņas kļūdas.</span><span class="sxs-lookup"><span data-stu-id="5cf44-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="5cf44-113">Piemērs:</span><span class="sxs-lookup"><span data-stu-id="5cf44-113">For example:</span></span>

<span data-ttu-id="5cf44-114">Šeit ir darbību centra ikona:</span><span class="sxs-lookup"><span data-stu-id="5cf44-114">Here's the Action Center icon:</span></span> ![Darbību centra ikona](media/action-center-icon.png) 

<span data-ttu-id="5cf44-116">Un paziņojuma paraugs:</span><span class="sxs-lookup"><span data-stu-id="5cf44-116">And a sample notification:</span></span> ![Nav atmiņas kļūdu](media/no-memory-errors.png)

<span data-ttu-id="5cf44-118">Ja esat izlaidis paziņojumu, uzdevumjoslā varat atlasīt **darbību centra** ikonu, lai parādītu **darbību centru** un skatītu ritināmo paziņojumu sarakstu.</span><span class="sxs-lookup"><span data-stu-id="5cf44-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="5cf44-119">Lai pārskatītu detalizētu informāciju, uzdevumjoslas meklēšanas lodziņā ierakstiet **notikums** un pēc tam atlasiet **notikumu skatītājs**.</span><span class="sxs-lookup"><span data-stu-id="5cf44-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="5cf44-120">**Notikumu skatītāja**kreisajā rūtī naviģējiet uz **Windows žurnālu > sistēmu**.</span><span class="sxs-lookup"><span data-stu-id="5cf44-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="5cf44-121">Labajā rūtī skenējiet sarakstu, aplūkojot **avota** kolonnu, līdz brīdim, kad tiek parādīts notikumi ar avota vērtību **memorydiagnostics-rezultāti**.</span><span class="sxs-lookup"><span data-stu-id="5cf44-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="5cf44-122">Izcelt katru šādu notikumu un redzēt rezultātu informāciju ailē zem cilnes **Vispārīgi** zem saraksta.</span><span class="sxs-lookup"><span data-stu-id="5cf44-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
