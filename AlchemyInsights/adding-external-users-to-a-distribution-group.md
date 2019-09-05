---
title: Ārējo lietotāju pievienošanu adresātu grupai
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: e84a5b04d6fc805deaa47cb10c91081f37411e5b
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737880"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="19f36-102">Ārējo lietotāju pievienošana adresātu grupai</span><span class="sxs-lookup"><span data-stu-id="19f36-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="19f36-103">Ārēja kontakta pievienošana adresātu grupai (DG) ir divpakāpju process:</span><span class="sxs-lookup"><span data-stu-id="19f36-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="19f36-104">Ārējā lietotāja pasta kontaktpersonas izveide:</span><span class="sxs-lookup"><span data-stu-id="19f36-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="19f36-105">Administrēšanas centrā atveriet lapu **lietotāju** > [kontaktpersonas](https://admin.microsoft.com/adminportal/home#/Contact) .</span><span class="sxs-lookup"><span data-stu-id="19f36-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="19f36-106">Atlasiet **Pievienot kontaktpersonu**.</span><span class="sxs-lookup"><span data-stu-id="19f36-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="19f36-107">Ierakstiet kontaktpersonas informāciju un atlasiet **pievienot**.</span><span class="sxs-lookup"><span data-stu-id="19f36-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="19f36-108">Pievienot pasta kontaktpersona jūsu ĢD:</span><span class="sxs-lookup"><span data-stu-id="19f36-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="19f36-109">Administrēšanas centrā pārejiet uz lapu **grupu** > [grupas.](https://admin.microsoft.com/adminportal/home#/groups)</span><span class="sxs-lookup"><span data-stu-id="19f36-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="19f36-110">Atrodiet ĢD, kuram vēlaties pievienot ārējo lietotāju, un atlasiet to, lai atvērtu rediģēšanas dialogu.</span><span class="sxs-lookup"><span data-stu-id="19f36-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="19f36-111">Cilnē **dalībnieki** atlasiet **Skatīt visu un pārvaldīt dalībniekus**.</span><span class="sxs-lookup"><span data-stu-id="19f36-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="19f36-112">Atlasiet vienumu **pievienot dalībniekus**.</span><span class="sxs-lookup"><span data-stu-id="19f36-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="19f36-113">Atlasiet iepriekšējā solī izveidoto pasta kontaktpersonu un pēc tam atlasiet **saglabāt**.</span><span class="sxs-lookup"><span data-stu-id="19f36-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="19f36-114">Ja pēc šīs darbības jūsu ārējie lietotāji nevar nosūtīt e-pastus DG vai nesaņem e-pastus no tā, tas varētu būt, ka ĢD ir atzīmēts atļaut tikai e-pastus no iekšējiem lietotājiem.</span><span class="sxs-lookup"><span data-stu-id="19f36-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="19f36-115">Jūs varat pārbaudīt šo konfigurāciju un noteikt to pēc virzienos [šeit](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="19f36-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="19f36-116">**Piezīme:** Šīs instrukcijas neattiecas, ja grupas tips ir "Office 365 grupas" nevis "adresātu grupa".</span><span class="sxs-lookup"><span data-stu-id="19f36-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="19f36-117">Šādā gadījumā ārējo lietotāju var pievienot tieši grupai no programmas Outlook.</span><span class="sxs-lookup"><span data-stu-id="19f36-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="19f36-118">Detalizēta informācija par Office 365 grupām viesi, kā arī instrukcijas, lai pievienotu ārējos viesi var atrast [šajā rakstā](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="19f36-118">Detailed information on Office 365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  