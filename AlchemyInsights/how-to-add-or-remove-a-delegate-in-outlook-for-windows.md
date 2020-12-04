---
title: Kā pievienot vai noņemt pārstāvi programmā Outlook darbam ar Windows
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573578"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a><span data-ttu-id="ab070-102">Kā pievienot vai noņemt pārstāvi programmā Outlook darbam ar Windows</span><span class="sxs-lookup"><span data-stu-id="ab070-102">How to add or remove a Delegate in Outlook for Windows</span></span>

<span data-ttu-id="ab070-103">Lai pievienotu pārstāvi programmā Outlook darbam ar Windows:</span><span class="sxs-lookup"><span data-stu-id="ab070-103">To add a Delegate in Outlook for Windows:</span></span> 

1. <span data-ttu-id="ab070-104">Noklikšķiniet uz cilnes **Fails** , pēc tam uz **konta iestatījumi** un pēc tam izvēlieties **pārstāvja piekļuve**.</span><span class="sxs-lookup"><span data-stu-id="ab070-104">Click on the **File** tab followed by **Account Settings**, and then choose **Delegate Access**.</span></span>
2. <span data-ttu-id="ab070-105">Noklikšķiniet uz **Pievienot**.</span><span class="sxs-lookup"><span data-stu-id="ab070-105">Click on **Add**.</span></span> <span data-ttu-id="ab070-106">Ja **pievienošana** netiek parādīta, iespējams, nepastāv aktīvs savienojums starp Outlook un Exchange.</span><span class="sxs-lookup"><span data-stu-id="ab070-106">If **Add** doesn’t appear, an active connection might not exist between Outlook and Exchange.</span></span> <span data-ttu-id="ab070-107">Outlook statusa joslā tiek rādīts savienojuma statuss.</span><span class="sxs-lookup"><span data-stu-id="ab070-107">The Outlook status bar displays the connection status.</span></span>
3. <span data-ttu-id="ab070-108">Ierakstiet tās personas vārdu, kuru vēlaties norādīt kā savu pārstāvi, vai meklējiet un sarakstā meklēšanas rezultāti izvēlieties vārdu.</span><span class="sxs-lookup"><span data-stu-id="ab070-108">Type the name of the person you want to designate as your delegate, or search and choose the name in the search results list.</span></span>

    > [!NOTE]
    > <span data-ttu-id="ab070-109">Pārstāvim ir jābūt personai, kas ir jūsu organizācijas Exchange globālajā adrešu sarakstā (GAL).</span><span class="sxs-lookup"><span data-stu-id="ab070-109">The delegate must be a person in your organization's Exchange Global Address List (GAL).</span></span>
4. <span data-ttu-id="ab070-110">Noklikšķiniet uz **Pievienot** un pēc tam uz **Labi**.</span><span class="sxs-lookup"><span data-stu-id="ab070-110">Click on **Add** followed by **OK**.</span></span>
5. <span data-ttu-id="ab070-111">Dialoglodziņā **pārstāvja atļaujas** akceptējiet noklusējuma atļauju iestatījumus vai atlasiet pielāgotus piekļuves līmeņus Exchange mapēm.</span><span class="sxs-lookup"><span data-stu-id="ab070-111">In the **Delegate Permissions** dialog box, accept the default permission settings or select custom access levels for Exchange folders.</span></span>

    - <span data-ttu-id="ab070-112">Ja pārstāvim ir nepieciešama atļauja darboties tikai ar sapulču pieprasījumiem un atbildēm, noklusējuma atļauju iestatījumi, piemēram, **pārstāvim, saņem man sūtīto sapulču ziņojumu kopijas** .</span><span class="sxs-lookup"><span data-stu-id="ab070-112">If a delegate needs permission to work only with meeting requests and responses, the default permission settings such as **Delegate receives copies of meeting-related messages sent to me** are sufficient.</span></span> <span data-ttu-id="ab070-113">Jūs varat atstāt **Iesūtnes** atļaujas iestatījumu **nevienā vietā.**</span><span class="sxs-lookup"><span data-stu-id="ab070-113">You can leave the **Inbox** permission setting at **None**.</span></span> <span data-ttu-id="ab070-114">Sapulču pieprasījumi un atbildes nonāk tieši pārstāvja iesūtnē.</span><span class="sxs-lookup"><span data-stu-id="ab070-114">Meeting requests and responses will go directly to the delegate's inbox.</span></span>

    > [!NOTE]
    > <span data-ttu-id="ab070-115">Pēc noklusējuma pārstāvim tiek piešķirts **redaktors (var lasīt, veidot un modificēt vienumus)** atļaujas jūsu **kalendāra** mapē.</span><span class="sxs-lookup"><span data-stu-id="ab070-115">By default, the delegate is granted **Editor (can read, create, and modify items)** permission to your **Calendar** folder.</span></span> <span data-ttu-id="ab070-116">Kad pārstāvis atbild uz sapulci jūsu vārdā, tas automātiski tiek pievienots jūsu **kalendāra** mapē.</span><span class="sxs-lookup"><span data-stu-id="ab070-116">When the delegate responds to a meeting on your behalf, it is automatically added to your **Calendar** folder.</span></span>

5. <span data-ttu-id="ab070-117">Lai nosūtītu ziņojumu, kas brīdina pārstāvi par izmaiņām atļaujās, atzīmējiet izvēles rūtiņu **automātiski nosūtīt pārstāvim ziņojumu, kurā apkopotas šīs atļaujas** .</span><span class="sxs-lookup"><span data-stu-id="ab070-117">To send a message to notify the delegate of the changed permissions, select the **Automatically send a message to delegate summarizing these permissions** check box.</span></span>
6. <span data-ttu-id="ab070-118">Ja vēlaties, atzīmējiet izvēles rūtiņu **pārstāvis var skatīt manus privātos vienumus** .</span><span class="sxs-lookup"><span data-stu-id="ab070-118">If you want, select the **Delegate can see my private items** check box.</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="ab070-119">Šis iestatījums ietekmē visas Exchange mapes.</span><span class="sxs-lookup"><span data-stu-id="ab070-119">This setting affects all Exchange folders.</span></span> <span data-ttu-id="ab070-120">Tas attiecas arī uz visām mapēm pasts, kontaktpersonas, kalendārs, uzdevumi, piezīmes un dienasgrāmata.</span><span class="sxs-lookup"><span data-stu-id="ab070-120">This includes all Mail, Contacts, Calendar, Tasks, Notes, and Journal folders.</span></span> <span data-ttu-id="ab070-121">Tikai norādītajās mapēs nav iespējams piešķirt piekļuvi privātajiem vienumiem.</span><span class="sxs-lookup"><span data-stu-id="ab070-121">There is no way to grant access to private items in only specified folders.</span></span>

7. <span data-ttu-id="ab070-122">Izvēlieties **Labi**.</span><span class="sxs-lookup"><span data-stu-id="ab070-122">Choose **OK**.</span></span>

    > [!NOTE]
    >
    > - <span data-ttu-id="ab070-123">Ziņojumi, kas nosūtīti, izmantojot atļaujas nosūtīt kā vārdā, ietver gan pārstāvja, gan jūsu vārdus blakus **no**.</span><span class="sxs-lookup"><span data-stu-id="ab070-123">Messages sent with Send on Behalf permissions include both the delegate's and your names next to **From**.</span></span> <span data-ttu-id="ab070-124">Kad ziņojums tiek sūtīts ar sūtīšanas atļaujām, parādās tikai jūsu vārds.</span><span class="sxs-lookup"><span data-stu-id="ab070-124">When a message is sent with Send As permissions, only your name appears.</span></span>
    > - <span data-ttu-id="ab070-125">Kad būsit pievienojis kādu personu kā pārstāvi, viņš var pievienot savu Exchange pastkasti savam Outlook profilam.</span><span class="sxs-lookup"><span data-stu-id="ab070-125">Once you add someone as a delegate, they can add your Exchange mailbox to their Outlook profile.</span></span> <span data-ttu-id="ab070-126">Norādījumus skatiet rakstā [citas personas pasta un kalendāra vienumu pārvaldība](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span><span class="sxs-lookup"><span data-stu-id="ab070-126">For instructions, see [Manage another person's mail and calendar items](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span></span>

<span data-ttu-id="ab070-127">Lai noņemtu pārstāvi programmā Outlook darbam ar Windows:</span><span class="sxs-lookup"><span data-stu-id="ab070-127">To remove a Delegate in Outlook for Windows:</span></span>

1. <span data-ttu-id="ab070-128">Noklikšķiniet uz cilnes **Fails** .</span><span class="sxs-lookup"><span data-stu-id="ab070-128">Click on the **File** tab.</span></span>
2. <span data-ttu-id="ab070-129">Noklikšķiniet uz **konta iestatījumi** un pēc tam uz **pārstāvja piekļuve**.</span><span class="sxs-lookup"><span data-stu-id="ab070-129">Click on **Account Settings** followed by **Delegate Access**.</span></span>
3. <span data-ttu-id="ab070-130">Izvēlieties tā pārstāvja vārdu, kuram vēlaties mainīt atļaujas, un pēc tam noklikšķiniet uz **Noņemt** , kam seko **Labi**.</span><span class="sxs-lookup"><span data-stu-id="ab070-130">Choose the name of the delegate for whom you want to change permissions, and then click on **Remove** followed by **OK**.</span></span>
