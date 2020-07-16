---
title: Attēlu ielādes problēmu novēršana pakalpojumā Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6000"
- "9003112"
ms.openlocfilehash: 93894eaa5818b591acd1c7b9a90bc1cabbe00450
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148291"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a><span data-ttu-id="a9e41-102">Attēlu ielādes problēmu novēršana pakalpojumā Yammer</span><span class="sxs-lookup"><span data-stu-id="a9e41-102">Troubleshoot image loading issues in Yammer</span></span>

<span data-ttu-id="a9e41-103">Ja rodas problēmas ar fotoattēliem un failu priekšskatījumi Yammer, novērst, pārbaudot, vai problēma rodas visiem lietotājiem, vai tas notiek mobilajās ierīcēs un vai tas ir reproducējams augšupielādējot pielikumu.</span><span class="sxs-lookup"><span data-stu-id="a9e41-103">When issues occur with photos and file previews in Yammer, troubleshoot by checking whether the issue occurs for all users, whether it occurs on mobile devices, and if it is reproducible when uploading the attachment.</span></span>  

<span data-ttu-id="a9e41-104">**Profila fotoattēlu problēmas**</span><span class="sxs-lookup"><span data-stu-id="a9e41-104">**Profile photo issues**</span></span>  

<span data-ttu-id="a9e41-105">Ja lietotāji pierakstās pakalpojumā Yammer, izmantojot Microsoft 365, viņiem ir jāmaina savs profils, tostarp profila fotoattēls.</span><span class="sxs-lookup"><span data-stu-id="a9e41-105">If end users sign into Yammer via Microsoft 365, they must change their profile, including their profile photo.</span></span> <span data-ttu-id="a9e41-106">Ja lietotājiem nav atļauts veikt profila atjauninājumus, administrators var veikt lietotāja atjauninājumu.</span><span class="sxs-lookup"><span data-stu-id="a9e41-106">If users are not permitted to make profile updates, an admin can make the update for the user.</span></span> <span data-ttu-id="a9e41-107">Papildinformāciju skatiet sadaļā [Profila skatīšana un atjaunināšana programmā Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="a9e41-107">For more info, see [View and update your profile in Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>

<span data-ttu-id="a9e41-108">Informāciju par profila rediģēšanu, tostarp profila fotoattēlus, skatiet [rakstā Yammer profila un iestatījumu mainīšana](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span><span class="sxs-lookup"><span data-stu-id="a9e41-108">For info about profile editing, including profile photos, see [Change my Yammer profile and settings](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span></span> 

<span data-ttu-id="a9e41-109">Atjauninātie profila fotoattēli tiek sinhronizēti citādi nekā profila atribūti.</span><span class="sxs-lookup"><span data-stu-id="a9e41-109">Updated profile photos are synced differently than profile attributes.</span></span> <span data-ttu-id="a9e41-110">Lietotājiem ir jāpierakstās, lai sāktu sava profila fotoattēla sinhronizāciju.</span><span class="sxs-lookup"><span data-stu-id="a9e41-110">Users must sign in to initiate a sync of their profile photo.</span></span> <span data-ttu-id="a9e41-111">Papildinformāciju skatiet sadaļā Lietotāja [profila attēli, kas atjaunināti no Office 365 uz Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span><span class="sxs-lookup"><span data-stu-id="a9e41-111">For info, see [are user profile pictures updated from Office 365 to Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span></span>

<span data-ttu-id="a9e41-112">Informāciju par lietotāja dzīves ciklu pakalpojumam Yammer skatiet rakstā [Yammer lietotāju pārvaldība visā viņu dzīves ciklā pakalpojumā Office 365.](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle)</span><span class="sxs-lookup"><span data-stu-id="a9e41-112">For info about the user lifecycle for Yammer, see [Manage Yammer users across their lifecycle from Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span></span>  

<span data-ttu-id="a9e41-113">Detalizētu informāciju par to, kā microsoft 365 darbojas profila attēlu sinhronizācija, skatiet [sadaļā Informācija par profila attēlu sinhronizāciju programmā Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span><span class="sxs-lookup"><span data-stu-id="a9e41-113">For details on how profile picture sync works in Microsoft 365, see [Information about profile picture synchronization in Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span></span>  

<span data-ttu-id="a9e41-114">**Dokumentu priekšskatījumi un attēlu sīktēlu problēmas**</span><span class="sxs-lookup"><span data-stu-id="a9e41-114">**Document previews and image thumbnail issues**</span></span>  

<span data-ttu-id="a9e41-115">Kad faili vai attēli tiek izlikti pakalpojumā Yammer, priekšskatījumi var neparādīties, jo:</span><span class="sxs-lookup"><span data-stu-id="a9e41-115">When files or images are posted to Yammer, previews might not appear because:</span></span> 

- <span data-ttu-id="a9e41-116">Fails ir bojāts, un to nevar apstrādāt.</span><span class="sxs-lookup"><span data-stu-id="a9e41-116">The file is corrupt and cannot be processed.</span></span>
- <span data-ttu-id="a9e41-117">Fails nav nesen augšupielādēts pakalpojumā SharePoint Online, vai Yammer ir nederīgi metadati citu iemeslu dēļ.</span><span class="sxs-lookup"><span data-stu-id="a9e41-117">The file has not been recently uploaded to SharePoint Online, or Yammer has invalid metadata for other reasons.</span></span>
- <span data-ttu-id="a9e41-118">Priekšskatījuma attēlu ielādei nepieciešamie vietrādis URL tiek bloķēti.</span><span class="sxs-lookup"><span data-stu-id="a9e41-118">URLs required for loading the preview images are blocked.</span></span>
- <span data-ttu-id="a9e41-119">Pirms grāmatošanas lietotājs noņēma faila priekšskatījumu.</span><span class="sxs-lookup"><span data-stu-id="a9e41-119">The file preview was removed by the user before posting.</span></span>
- <span data-ttu-id="a9e41-120">Pakalpojuma problēma neļāva ģenerēt priekšskatījumu.</span><span class="sxs-lookup"><span data-stu-id="a9e41-120">A service issue prevented a preview being generated.</span></span>

<span data-ttu-id="a9e41-121">**Piezīme:** Saišu un failu augšupielādes priekšskatījumi var uzveikt citādi.</span><span class="sxs-lookup"><span data-stu-id="a9e41-121">**Note** Previews for links and file uploads might behave differently.</span></span> <span data-ttu-id="a9e41-122">Saites uz failiem internetā vai saites, kurām nepieciešama papildu autentifikācija, iespējams, netiks rādītas pareizi.</span><span class="sxs-lookup"><span data-stu-id="a9e41-122">Links to files on the internet or links that require additional authentication might not display correctly.</span></span>

<span data-ttu-id="a9e41-123">Papildinformāciju skatiet rakstā [Faila vai attēla pievienošana Yammer ziņojumam](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span><span class="sxs-lookup"><span data-stu-id="a9e41-123">For more info, see [Attach a file or image to a Yammer message](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span></span> 