---
title: Paroļu atpakaļrakstīšanas iespējošana Azure AD Connect
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
- "9002933"
- "5615"
ms.openlocfilehash: 2ad7568bded3c8e4832e0e433a2d715e6307e4bb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814019"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="921cc-102">Paroļu atpakaļrakstīšanas iespējošana Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="921cc-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="921cc-103">Lai iespējotu patstāvīgi izmantojamu paroles atiestatīšanas atpakaļrakstīšanu, vispirms Azure AD Connect iespējojiet atpakaļrakstīšanas opciju.</span><span class="sxs-lookup"><span data-stu-id="921cc-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="921cc-104">Savā Azure AD Connect serverī veiciet tālāk minētās darbības:</span><span class="sxs-lookup"><span data-stu-id="921cc-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="921cc-105">Pierakstieties savā AD Connect serverī un palaidiet **Azure AD Connect** konfigurēšanas vedni.</span><span class="sxs-lookup"><span data-stu-id="921cc-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="921cc-106">**Sākuma** lapā noklikšķiniet uz **Konfigurēt**.</span><span class="sxs-lookup"><span data-stu-id="921cc-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="921cc-107">**Papildu uzdevumu** lapā atlasiet **Pielāgot sinhronizācijas opcijas** un noklikšķiniet uz **Tālāk**.</span><span class="sxs-lookup"><span data-stu-id="921cc-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="921cc-108">Lapā **Izveidot savienojumu ar Azure AD**, ievadiet jūsu Azure nomnieka globālā administratora akreditācijas datus un pēc tam noklikšķiniet **Tālāk**.</span><span class="sxs-lookup"><span data-stu-id="921cc-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="921cc-109">Filtrēšanas lapās **Connect direktoriji** un **Domēns/OU** noklikšķiniet uz **Tālāk**.</span><span class="sxs-lookup"><span data-stu-id="921cc-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="921cc-110">Lapā **Papildu līdzekļi**, atlasiet rūtiņu pie **Paroles atpakaļrakstīšana** un noklikšķiniet uz **Tālāk**.</span><span class="sxs-lookup"><span data-stu-id="921cc-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="921cc-111">Lapā **Gatavs konfigurēšanai** noklikšķiniet uz **Konfigurēt** un sagaidiet procesa beigas.</span><span class="sxs-lookup"><span data-stu-id="921cc-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="921cc-112">Kad tiks parādīta konfigurācija, noklikšķiniet uz **Iziet**.</span><span class="sxs-lookup"><span data-stu-id="921cc-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="921cc-113">Kad Azure AD Connect paroles atpakaļrakstīšana ir iespējota, konfigurējiet Azure AD SSPR atpakaļrakstīšanai.</span><span class="sxs-lookup"><span data-stu-id="921cc-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="921cc-114">Lai iespējotu SSPR paroles atpakaļrakstīšanu, veiciet tālāk minētās darbības: </span><span class="sxs-lookup"><span data-stu-id="921cc-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="921cc-115">Ierakstieties Azure portālā ar globālā administratora kontu.</span><span class="sxs-lookup"><span data-stu-id="921cc-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="921cc-116">Meklējiet un atlasiet **Azure Active Directory**, noklikšķiniet uz **Paroles atiestatīšana**, pēc tam noklikšķiniet uz **Lokālā integrācija**.</span><span class="sxs-lookup"><span data-stu-id="921cc-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="921cc-117">Iestatiet opciju **Veikt paroļu atpakaļrakstīšanu jūsu lokālajam direktorijam?** kā **Jā**.</span><span class="sxs-lookup"><span data-stu-id="921cc-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="921cc-118">Iestatiet opciju **Ļaut lietotājiem atbloķēt kontus bez paroļu atiestatīšanas?** kā **Jā**.</span><span class="sxs-lookup"><span data-stu-id="921cc-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="921cc-119">Pēc tam noklikšķiniet uz **Saglabāt**.</span><span class="sxs-lookup"><span data-stu-id="921cc-119">When ready, click **Save**.</span></span>

<span data-ttu-id="921cc-120">Papildinformācijai lasiet [Azure Active Directory patstāvīgās paroles atiestatīšanas atpakaļrakstīšanas iespējošana lokālajā vidē](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="921cc-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="921cc-121">Kad administrators atiestata lietotāja paroli Azure portālā, ja lietotājs ir federatīvs vai parole ir sinhronizēta ar jaucējkodu, parole tiek lokāli atpakļrakstīta.</span><span class="sxs-lookup"><span data-stu-id="921cc-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="921cc-122">Šai funkcionalitātei ir nepieciešama Azure Premium licence (P1 vai P2), un tā pašlaik netiek atbalstīta Office administratora portālā.</span><span class="sxs-lookup"><span data-stu-id="921cc-122">This functionality requires Azure Premium License (P1 or P2) and is currently not supported in the Office Admin portal.</span></span>
