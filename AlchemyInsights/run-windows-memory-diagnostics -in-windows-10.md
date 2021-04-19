---
title: Windows atmiņas diagnostikas palaišana operētājsistēmā Windows 10
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
- "9002959"
- "5661"
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826674"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="399c3-102">Windows atmiņas diagnostikas palaišana operētājsistēmā Windows 10</span><span class="sxs-lookup"><span data-stu-id="399c3-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="399c3-103">Ja jūsu datorā operētājsistēma Windows un programmas avarē, sasalst vai darbojas nestabilā veidā, iespējams, radusies problēma ar datora atmiņu (RAM).</span><span class="sxs-lookup"><span data-stu-id="399c3-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="399c3-104">Varat palaist Windows atmiņas diagnostiku, lai meklētu problēmas saistībā ar datora RAM.</span><span class="sxs-lookup"><span data-stu-id="399c3-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="399c3-105">Uzdevumjoslas meklēšanas lodziņā ierakstiet atmiņas **diagnostika un** pēc tam atlasiet **Windows atmiņas diagnostika**.</span><span class="sxs-lookup"><span data-stu-id="399c3-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="399c3-106">Lai palaistu diagnostiku, dators ir jārestartē.</span><span class="sxs-lookup"><span data-stu-id="399c3-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="399c3-107">Varat restartēt tūlīt (lūdzu, vispirms saglabāt savu darbu un aizvērt atvērtos dokumentus un e-pasta ziņojumus) vai ieplānot diagnostikas automātisku pašanu nākamajā datora restartēšanas reizē:</span><span class="sxs-lookup"><span data-stu-id="399c3-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Windows atmiņas diagnostika](media/windows-memory-diagnostic.png)

<span data-ttu-id="399c3-109">Pēc datora restartēšanas automātiski tiek **palaists Windows atmiņas diagnostikas** rīks.</span><span class="sxs-lookup"><span data-stu-id="399c3-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="399c3-110">Statuss un norise tiks parādītas, palaižot diagnostiku, un jums ir iespēja  atcelt diagnostiku, nospiežot tastatūras taustiņu ESC.</span><span class="sxs-lookup"><span data-stu-id="399c3-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="399c3-111">Kad diagnostika ir pabeigta, Windows tiks startēta kā parasti.</span><span class="sxs-lookup"><span data-stu-id="399c3-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="399c3-112">Uzreiz pēc restartēšanas, kad tiek parādīta darbvirsma,  uzdevumjoslā tiek parādīts paziņojums (blakus darbību centra ikonai), lai norādītu, vai ir atrastas atmiņas kļūdas.</span><span class="sxs-lookup"><span data-stu-id="399c3-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="399c3-113">Piemēram:</span><span class="sxs-lookup"><span data-stu-id="399c3-113">For example:</span></span>

<span data-ttu-id="399c3-114">Tālāk ir redzama darbību centra ikona.</span><span class="sxs-lookup"><span data-stu-id="399c3-114">Here's the Action Center icon:</span></span> ![Darbību centra ikona](media/action-center-icon.png) 

<span data-ttu-id="399c3-116">Un paziņojuma paraugs:</span><span class="sxs-lookup"><span data-stu-id="399c3-116">And a sample notification:</span></span> ![Atmiņas kļūdu nav](media/no-memory-errors.png)

<span data-ttu-id="399c3-118">Ja nepamanīāt paziņojumu,  varat atlasīt darbību centra ikonu  uzdevumjoslā, lai atvērtu darbību centru un skatītu ritināmu paziņojumu sarakstu.</span><span class="sxs-lookup"><span data-stu-id="399c3-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="399c3-119">Lai pārskatītu detalizētu informāciju, **ierakstiet notikums** uzdevumjoslas meklēšanas lodziņā un pēc tam atlasiet **Notikumu skatītājs**.</span><span class="sxs-lookup"><span data-stu-id="399c3-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="399c3-120">Notikumu **skatītāja** kreisajā rūtī naviģējiet uz **Windows žurnālus > sistēmu**.</span><span class="sxs-lookup"><span data-stu-id="399c3-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="399c3-121">Labajā rūtī noskenējiet sarakstu, vienlaikus aplūkojot kolonnu Avots, līdz tiek atvērts notikums ar avota vērtību **MemoryDiagnostics-Results.** </span><span class="sxs-lookup"><span data-stu-id="399c3-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="399c3-122">Iezīmējiet katru šādu notikumu un skatiet rezultātu informāciju lodziņā zem **cilnes** Vispārīgi zem saraksta.</span><span class="sxs-lookup"><span data-stu-id="399c3-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
