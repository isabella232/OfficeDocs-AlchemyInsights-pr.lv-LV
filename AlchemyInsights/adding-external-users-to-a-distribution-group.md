---
title: Ārējo lietotāju pievienošana adresātu grupai
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663520"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="d0bda-102">Ārējo lietotāju pievienošana adresātu grupai</span><span class="sxs-lookup"><span data-stu-id="d0bda-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="d0bda-103">Ārējas kontaktpersonas pievienošana adresātu grupai (DG) ir divu soļu process:</span><span class="sxs-lookup"><span data-stu-id="d0bda-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="d0bda-104">Izveidojiet pasta kontaktpersonu ārējam lietotājam:</span><span class="sxs-lookup"><span data-stu-id="d0bda-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="d0bda-105">Administrēšanas centrā dodieties uz lapu **lietotāju**  >  [kontaktpersonas](https://admin.microsoft.com/adminportal/home#/Contact) .</span><span class="sxs-lookup"><span data-stu-id="d0bda-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="d0bda-106">Atlasiet **Pievienot kontaktpersonu**.</span><span class="sxs-lookup"><span data-stu-id="d0bda-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="d0bda-107">Ierakstiet kontaktpersonas informāciju un atlasiet **Pievienot**.</span><span class="sxs-lookup"><span data-stu-id="d0bda-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="d0bda-108">Pievienojiet pasta kontaktpersonu savam ĢENERĀLDIREKTORĀTAm:</span><span class="sxs-lookup"><span data-stu-id="d0bda-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="d0bda-109">Administrēšanas centrā dodieties uz lapu **grupu**  >  [grupas](https://admin.microsoft.com/adminportal/home#/groups) .</span><span class="sxs-lookup"><span data-stu-id="d0bda-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="d0bda-110">Atrodiet DG, kuram vēlaties pievienot ārējo lietotāju, un atlasiet to, lai atvērtu rediģēšanas dialoglodziņu.</span><span class="sxs-lookup"><span data-stu-id="d0bda-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="d0bda-111">Cilnē **dalībnieki** atlasiet **Skatīt visus un pārvaldīt dalībniekus**.</span><span class="sxs-lookup"><span data-stu-id="d0bda-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="d0bda-112">Atlasiet **Pievienot dalībniekus**.</span><span class="sxs-lookup"><span data-stu-id="d0bda-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="d0bda-113">Atlasiet iepriekšējā darbībā izveidoto pasta kontaktpersonu un pēc tam atlasiet **Saglabāt**.</span><span class="sxs-lookup"><span data-stu-id="d0bda-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="d0bda-114">Ja pēc šo darbību veikšanas ārējie lietotāji nevar nosūtīt e-pasta ziņojumus uz DG vai nesaņem e-pasta ziņojumus no šīs darbības, iespējams, ka DG ir atzīmēts atļaut tikai e-pasta ziņojumus no iekšējiem lietotājiem.</span><span class="sxs-lookup"><span data-stu-id="d0bda-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="d0bda-115">Varat pārbaudīt šo konfigurāciju un izlabot to, sekojot norādījumiem, kas sniegti [šeit](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="d0bda-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="d0bda-116">**Piezīme:** Šīs instrukcijas nav spēkā, ja jūsu grupas tips ir "Microsoft 365 Group", nevis "adresātu grupa".</span><span class="sxs-lookup"><span data-stu-id="d0bda-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="d0bda-117">Šādā gadījumā ārējo lietotāju varat pievienot tieši grupai no Outlook.</span><span class="sxs-lookup"><span data-stu-id="d0bda-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="d0bda-118">Detalizētu informāciju par Microsoft 365 grupām viesi, kā arī norādījumus par ārējo viesu pievienošanu, var skatīt [šajā rakstā](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="d0bda-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  