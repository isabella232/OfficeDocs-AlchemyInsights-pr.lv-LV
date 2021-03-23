---
title: Importēšana un eksportēšana no Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036122"
---
# <a name="import-and-export-from-yammer"></a><span data-ttu-id="e945f-102">Importēšana un eksportēšana no Yammer</span><span class="sxs-lookup"><span data-stu-id="e945f-102">Import and export from Yammer</span></span>

<span data-ttu-id="e945f-103">**Importa**</span><span class="sxs-lookup"><span data-stu-id="e945f-103">**Import**</span></span>

<span data-ttu-id="e945f-104">Lietotāja importēšanas opcijas atšķiras atkarībā no tā, vai jūsu Yammer tīkls ir [Microsoft 365 vietējā režīmā](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode).</span><span class="sxs-lookup"><span data-stu-id="e945f-104">User-import options vary depending on whether your Yammer network is in [Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), or not.</span></span>

- <span data-ttu-id="e945f-105">**Nevietējais režīms**: lietotājus var importēt grupās, izmantojot opciju [Pievienot no adrešu grāmatas](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (ierobežot līdz 100 lietotājiem) grupas iestatījumos vai tīklā, izmantojot [lielapjoma atjaunināšanu](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) tīkla administrators.</span><span class="sxs-lookup"><span data-stu-id="e945f-105">**Non-Native Mode**: Users can be imported to groups using [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limit to 100 users) within group settings, or to the network using [Bulk Update](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) within Network Admin.</span></span>
- <span data-ttu-id="e945f-106">**Vietējais režīms**: dalības grupas un tīkla dalības darbības jāveic no [Microsoft 365 administrēšanas portāla](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portāla](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)vai izmantojot citu Azure AD opciju.</span><span class="sxs-lookup"><span data-stu-id="e945f-106">**Native Mode**: Group membership and network membership operations should be performed from the [Microsoft 365 admin portal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), or using another Azure AD option.</span></span> <span data-ttu-id="e945f-107">Vietējā režīmā tīkliem vairs nav pieejama lielapjoma atjaunināšana un citi mantotie līdzekļi.</span><span class="sxs-lookup"><span data-stu-id="e945f-107">Networks in Native Mode no longer have access to Bulk Update and other legacy features.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="e945f-108">Yammer nekad neatbalsta satura importēšanu no tīkla administratora pat tad, ja datu eksportēšanas līdzeklis ir izmantots citā tīklā.</span><span class="sxs-lookup"><span data-stu-id="e945f-108">Yammer never supported importing content from within Network Admin even when the Data Export feature was used in another network.</span></span> <span data-ttu-id="e945f-109">Saturu var atkārtoti publicēt partnera risinājumos vai Yammer REST API.</span><span class="sxs-lookup"><span data-stu-id="e945f-109">Content can be re-posted by partner solutions or the Yammer REST APIs.</span></span>

<span data-ttu-id="e945f-110">**Eksportēšana**</span><span class="sxs-lookup"><span data-stu-id="e945f-110">**Export**</span></span>

<span data-ttu-id="e945f-111">Tīkla [datu eksportēšana tīkla administrators](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) ļauj eksportēt saturu no Yammer tīkliem, tostarp ziņojumiem un failiem.</span><span class="sxs-lookup"><span data-stu-id="e945f-111">[Export Network Data within Network Admin](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permits the export of content from Yammer networks, including messages and files.</span></span> <span data-ttu-id="e945f-112">Pielikumi var būt ļoti lieli, un to veikšanai būs nepieciešams ievērojams laiks.</span><span class="sxs-lookup"><span data-stu-id="e945f-112">Attachments can be extremely large and will cause exports to take significant time to complete.</span></span> <span data-ttu-id="e945f-113">Ir ieteicams, lai aktīvie tīkli tiktu eksportēti, izmantojot [datu eksportēšanas API](https://developer.yammer.com/docs/data-export-api) , kas atrodas gabalos pēc dienas vai nedēļas.</span><span class="sxs-lookup"><span data-stu-id="e945f-113">We recommend that active networks are exported using the [Data Export API](https://developer.yammer.com/docs/data-export-api) in chunks by day or week.</span></span> <span data-ttu-id="e945f-114">Microsoft atbalsts šim nolūkam nenodrošina pielāgotus skriptus.</span><span class="sxs-lookup"><span data-stu-id="e945f-114">Microsoft Support does not provide custom scripts for this purpose.</span></span>

<span data-ttu-id="e945f-115">Pastāv atsevišķs [vdar eksports](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) , lai eksportētu saturu atsevišķam lietotājam.</span><span class="sxs-lookup"><span data-stu-id="e945f-115">A separate [GDPR export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) exists to export content for an individual user.</span></span>