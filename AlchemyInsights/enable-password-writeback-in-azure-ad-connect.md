---
title: Paroļu atpakaļrakstīšanas iespējošana Azure AD Connect
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 1e90aedab20c8abaa021ed980e868cea0503b7b1
ms.sourcegitcommit: db95fd628c45d9810e5af5c5a4e6388c793339ac
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093362"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="1e1fc-102">Paroļu atpakaļrakstīšanas iespējošana Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="1e1fc-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="1e1fc-103">Lai iespējotu patstāvīgi izmantojamu paroles atiestatīšanas atpakaļrakstīšanu, vispirms Azure AD Connect iespējojiet atpakaļrakstīšanas opciju.</span><span class="sxs-lookup"><span data-stu-id="1e1fc-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="1e1fc-104">Savā Azure AD Connect serverī veiciet tālāk minētās darbības:</span><span class="sxs-lookup"><span data-stu-id="1e1fc-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="1e1fc-105">Pierakstieties savā AD Connect serverī un palaidiet **Azure AD Connect** konfigurēšanas vedni.</span><span class="sxs-lookup"><span data-stu-id="1e1fc-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="1e1fc-106">**Sākuma** lapā noklikšķiniet uz **Konfigurēt**.</span><span class="sxs-lookup"><span data-stu-id="1e1fc-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="1e1fc-107">**Papildu uzdevumu** lapā atlasiet **Pielāgot sinhronizācijas opcijas** un noklikšķiniet uz **Tālāk**.</span><span class="sxs-lookup"><span data-stu-id="1e1fc-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="1e1fc-108">Lapā **Izveidot savienojumu ar Azure AD**, ievadiet jūsu Azure nomnieka globālā administratora akreditācijas datus un pēc tam noklikšķiniet **Tālāk**.</span><span class="sxs-lookup"><span data-stu-id="1e1fc-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="1e1fc-109">Filtrēšanas lapās **Connect direktoriji** un **Domēns/OU** noklikšķiniet uz **Tālāk**.</span><span class="sxs-lookup"><span data-stu-id="1e1fc-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="1e1fc-110">Lapā **Papildu līdzekļi**, atlasiet rūtiņu pie **Paroles atpakaļrakstīšana** un noklikšķiniet uz **Tālāk**.</span><span class="sxs-lookup"><span data-stu-id="1e1fc-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="1e1fc-111">Lapā **Gatavs konfigurēšanai** noklikšķiniet uz **Konfigurēt** un sagaidiet procesa beigas.</span><span class="sxs-lookup"><span data-stu-id="1e1fc-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="1e1fc-112">Kad tiks parādīta konfigurācija, noklikšķiniet uz **Iziet**.</span><span class="sxs-lookup"><span data-stu-id="1e1fc-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="1e1fc-113">Kad Azure AD Connect paroles atpakaļrakstīšana ir iespējota, konfigurējiet Azure AD SSPR atpakaļrakstīšanai.</span><span class="sxs-lookup"><span data-stu-id="1e1fc-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="1e1fc-114">Lai iespējotu SSPR paroles atpakaļrakstīšanu, veiciet tālāk minētās darbības: </span><span class="sxs-lookup"><span data-stu-id="1e1fc-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="1e1fc-115">Ierakstieties Azure portālā ar globālā administratora kontu.</span><span class="sxs-lookup"><span data-stu-id="1e1fc-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="1e1fc-116">Meklējiet un atlasiet **Azure Active Directory**, noklikšķiniet uz **Paroles atiestatīšana**, pēc tam noklikšķiniet uz **Lokālā integrācija**.</span><span class="sxs-lookup"><span data-stu-id="1e1fc-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="1e1fc-117">Iestatiet opciju **Veikt paroļu atpakaļrakstīšanu jūsu lokālajam direktorijam?** kā **Jā**.</span><span class="sxs-lookup"><span data-stu-id="1e1fc-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="1e1fc-118">Iestatiet opciju **Ļaut lietotājiem atbloķēt kontus bez paroļu atiestatīšanas?** kā **Jā**.</span><span class="sxs-lookup"><span data-stu-id="1e1fc-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="1e1fc-119">Pēc tam noklikšķiniet uz **Saglabāt**.</span><span class="sxs-lookup"><span data-stu-id="1e1fc-119">When ready, click **Save**.</span></span>

<span data-ttu-id="1e1fc-120">Papildinformācijai lasiet [Azure Active Directory patstāvīgās paroles atiestatīšanas atpakaļrakstīšanas iespējošana lokālajā vidē](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="1e1fc-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="1e1fc-121">Kad administrators atiestata lietotāja paroli Azure portālā, ja lietotājs ir federatīvs vai parole ir sinhronizēta ar jaucējkodu, parole tiek lokāli atpakļrakstīta.</span><span class="sxs-lookup"><span data-stu-id="1e1fc-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="1e1fc-122">Šai funkcionalitātei ir nepieciešama Azure Premium licence (P1 vai P2), un tā pašlaik netiek atbalstīta Office administratora portālā.</span><span class="sxs-lookup"><span data-stu-id="1e1fc-122">This functionality requires Azure Premium License (P1 or P2) and is currently not supported in the Office Admin portal.</span></span>
