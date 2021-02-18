---
title: Ārējo iestatījumu pārvaldība
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8322"
- "9003227"
ms.openlocfilehash: 7caf46f9988ddbcbb16c0a2751dbda85bd7da34c
ms.sourcegitcommit: 616ae0cbd5769e12ae428e00088840cf05e52b6a
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/17/2021
ms.locfileid: "50294316"
---
# <a name="managing-external-settings"></a><span data-ttu-id="ce85d-102">Ārējo iestatījumu pārvaldība</span><span class="sxs-lookup"><span data-stu-id="ce85d-102">Managing External Settings</span></span>

<span data-ttu-id="ce85d-103">**Paziņojums**</span><span class="sxs-lookup"><span data-stu-id="ce85d-103">**Announcement**</span></span>

- <span data-ttu-id="ce85d-104">Tīmekļa [skata pierakstīšanās atbalsts no Google, sākot ar 4. janvāri, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span><span class="sxs-lookup"><span data-stu-id="ce85d-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span></span> <span data-ttu-id="ce85d-105">Pārbaudiet, vai jūsu lietojumprogrammas ir skārusi, ievērojot Google norādījumus par saderības testēšanu</span><span class="sxs-lookup"><span data-stu-id="ce85d-105">Test whether your apps are affected by following Google’s guidance on testing compatibility</span></span>
- <span data-ttu-id="ce85d-106">Pierakstoties lietotājiem ar patēriņa Google kontiem, noteikti izmantojiet sistēmas tīmekļa skatu vai sistēmas pārlūkprogrammu</span><span class="sxs-lookup"><span data-stu-id="ce85d-106">Make sure to use the system webview or the system browser when signing in your users with consumer Google accounts</span></span>

<span data-ttu-id="ce85d-107">**Uzaicinājuma iestatījumu pārvaldība**</span><span class="sxs-lookup"><span data-stu-id="ce85d-107">**Manage Invitation Settings**</span></span>

<span data-ttu-id="ce85d-108">Pārliecinieties, vai esat [konfigurējis ārējos sadarbības iestatījumus](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) tā, lai ļautu attiecīgajām personām nosūtīt uzaicinājumus.</span><span class="sxs-lookup"><span data-stu-id="ce85d-108">Confirm that you have [configured the external collaboration settings](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) to allow the appropriate people to send invitations.</span></span>

<span data-ttu-id="ce85d-109">**Vieslietotāju piekļuves atļauju pārvaldība**</span><span class="sxs-lookup"><span data-stu-id="ce85d-109">**Manage Guest User Access Permissions**</span></span>

1. <span data-ttu-id="ce85d-110">Globālie administratori var pārvaldīt viesu piekļuves atļaujas direktorijā, izmantojot Azure portālu, konfigurējot viesa piekļuves atļaujas ārējas sadarbības iestatījumu lapā.</span><span class="sxs-lookup"><span data-stu-id="ce85d-110">Global admins can manage guest access permissions in the directory through the Azure portal by configuring the guest access permissions on the External Collaboration Settings page.</span></span> <span data-ttu-id="ce85d-111">[Uzziniet vairāk par šo iestatījumu](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="ce85d-111">[Learn more about this setting](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
2. <span data-ttu-id="ce85d-112">Ja vēlaties, lai jūsu viesi varētu piekļūt programmām, piemēram, Teams vai SharePoint, apstipriniet, ka šīs lietojumprogrammas ir konfigurētas, lai atļautu viesu piekļuvi.</span><span class="sxs-lookup"><span data-stu-id="ce85d-112">If you would like your guests to access apps such as Teams or SharePoint, confirm that you've configured those apps to allow guest access.</span></span> <span data-ttu-id="ce85d-113">Uzziniet vairāk par [grupu iestatījumiem](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) un [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="ce85d-113">Learn more about the [Teams settings](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) and [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="ce85d-114">**Uzaicinājumu konfigurēšana:**</span><span class="sxs-lookup"><span data-stu-id="ce85d-114">**Configuring invitations:**</span></span>

- [<span data-ttu-id="ce85d-115">Iespējot B2B ārējo sadarbību un pārvaldīt lietotājus, kas var uzaicināt viesus</span><span class="sxs-lookup"><span data-stu-id="ce85d-115">Enable B2B external collaboration and manage who can invite guests</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="ce85d-116">Ielūgumu atļaušana vai bloķēšana konkrētu organizāciju lietotājiem</span><span class="sxs-lookup"><span data-stu-id="ce85d-116">Allow or block invitations to users from specific organizations</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="ce85d-117">**Atļauto identitātes nodrošinātāju konfigurēšana**</span><span class="sxs-lookup"><span data-stu-id="ce85d-117">**Configuring allowed identity providers:**</span></span>

- [<span data-ttu-id="ce85d-118">Google Federācija</span><span class="sxs-lookup"><span data-stu-id="ce85d-118">Google Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="ce85d-119">Tieša Federācija</span><span class="sxs-lookup"><span data-stu-id="ce85d-119">Direct Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="ce85d-120">Vienreizējas patentatslēgas autentifikācija pa e-pastu</span><span class="sxs-lookup"><span data-stu-id="ce85d-120">Email one-time Passcode Authentication</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)
