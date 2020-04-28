---
title: Ārējo lietotāju pievienošanu adresātu grupai
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 7dbc69bced9ca800d3f95081b77dda5e49662579
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/27/2020
ms.locfileid: "43910939"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="4f2ad-102">Ārējo lietotāju pievienošana adresātu grupai</span><span class="sxs-lookup"><span data-stu-id="4f2ad-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="4f2ad-103">Ārēja kontakta pievienošana adresātu grupai (DG) ir divpakāpju process:</span><span class="sxs-lookup"><span data-stu-id="4f2ad-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="4f2ad-104">Ārējā lietotāja pasta kontaktpersonas izveide:</span><span class="sxs-lookup"><span data-stu-id="4f2ad-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="4f2ad-105">Administrēšanas centrā atveriet lapu **lietotāju** > [kontaktpersonas](https://admin.microsoft.com/adminportal/home#/Contact) .</span><span class="sxs-lookup"><span data-stu-id="4f2ad-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="4f2ad-106">Atlasiet **Pievienot kontaktpersonu**.</span><span class="sxs-lookup"><span data-stu-id="4f2ad-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="4f2ad-107">Ierakstiet kontaktpersonas informāciju un atlasiet **pievienot**.</span><span class="sxs-lookup"><span data-stu-id="4f2ad-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="4f2ad-108">Pievienot pasta kontaktpersona jūsu ĢD:</span><span class="sxs-lookup"><span data-stu-id="4f2ad-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="4f2ad-109">Administrēšanas centrā pārejiet uz lapu **grupu** > [grupas.](https://admin.microsoft.com/adminportal/home#/groups)</span><span class="sxs-lookup"><span data-stu-id="4f2ad-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="4f2ad-110">Atrodiet ĢD, kuram vēlaties pievienot ārējo lietotāju, un atlasiet to, lai atvērtu rediģēšanas dialogu.</span><span class="sxs-lookup"><span data-stu-id="4f2ad-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="4f2ad-111">Cilnē **dalībnieki** atlasiet **Skatīt visu un pārvaldīt dalībniekus**.</span><span class="sxs-lookup"><span data-stu-id="4f2ad-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="4f2ad-112">Atlasiet vienumu **pievienot dalībniekus**.</span><span class="sxs-lookup"><span data-stu-id="4f2ad-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="4f2ad-113">Atlasiet iepriekšējā solī izveidoto pasta kontaktpersonu un pēc tam atlasiet **saglabāt**.</span><span class="sxs-lookup"><span data-stu-id="4f2ad-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="4f2ad-114">Ja pēc šīs darbības jūsu ārējie lietotāji nevar nosūtīt e-pastus DG vai nesaņem e-pastus no tā, tas varētu būt, ka ĢD ir atzīmēts atļaut tikai e-pastus no iekšējiem lietotājiem.</span><span class="sxs-lookup"><span data-stu-id="4f2ad-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="4f2ad-115">Jūs varat pārbaudīt šo konfigurāciju un noteikt to pēc virzienos [šeit](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="4f2ad-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="4f2ad-116">**Piezīme:** Šīs instrukcijas neattiecas, ja grupas tips ir "Microsoft 365 grupas" nevis "adresātu grupas".</span><span class="sxs-lookup"><span data-stu-id="4f2ad-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="4f2ad-117">Šādā gadījumā ārējo lietotāju var pievienot tieši grupai no programmas Outlook.</span><span class="sxs-lookup"><span data-stu-id="4f2ad-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="4f2ad-118">Detalizēta informācija par Microsoft 365 grupām viesi, kā arī instrukcijas, lai pievienotu ārējos viesi var atrast [šajā rakstā](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="4f2ad-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  