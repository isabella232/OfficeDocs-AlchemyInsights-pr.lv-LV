---
title: Problēmu novēršanas notikumus no e-pasta
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569138"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="af968-102">Problēmu novēršanas notikumus no e-pasta</span><span class="sxs-lookup"><span data-stu-id="af968-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="af968-103">Pārbaudiet, vai ir iespējots līdzeklis pastkastes: \*\*Get EventsFromEmailConfiguration-identitātes <mailbox> \*\*</span><span class="sxs-lookup"><span data-stu-id="af968-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="af968-104">Pēc tam apskatiet "notikumus no e-pasta" žurnālus **Export-MailboxDiagnosticLogs <mailbox> -komponenta timeprofile**</span><span class="sxs-lookup"><span data-stu-id="af968-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="af968-105">Žurnālos "notikumi no e-pasta" atrodiet InternetMessageId, kas atbilst pastkastes vienumam.</span><span class="sxs-lookup"><span data-stu-id="af968-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="af968-106">TrustScore nosaka, vai krājums ir pievienots vai nav.</span><span class="sxs-lookup"><span data-stu-id="af968-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="af968-107">Notikumi tiks pievienoti tikai tad, ja TrustScore = "uzticams".</span><span class="sxs-lookup"><span data-stu-id="af968-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="af968-108">TrustScore nosaka ar SPF, DKIM vai Dmarc rekvizītiem, kas atrodas ziņojuma galvenē.</span><span class="sxs-lookup"><span data-stu-id="af968-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="af968-109">Lai skatītu šos rekvizītus:</span><span class="sxs-lookup"><span data-stu-id="af968-109">To view these properties:</span></span>

<span data-ttu-id="af968-110">**Desktop Outlook**</span><span class="sxs-lookup"><span data-stu-id="af968-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="af968-111">Atveriet vienumu</span><span class="sxs-lookup"><span data-stu-id="af968-111">Open the item</span></span>
- <span data-ttu-id="af968-112">Fails-> rekvizīti-> interneta galvenes</span><span class="sxs-lookup"><span data-stu-id="af968-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="af968-113">Vai</span><span class="sxs-lookup"><span data-stu-id="af968-113">or</span></span>

<span data-ttu-id="af968-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="af968-114">**MFCMapi**</span></span>

- <span data-ttu-id="af968-115">Naviģējiet uz vienumu iesūtnē</span><span class="sxs-lookup"><span data-stu-id="af968-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="af968-116">Meklēt PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="af968-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="af968-117">Šie rekvizīti tiek noteikti un reģistrēti transportēšanas un maršrutēšanas laikā.</span><span class="sxs-lookup"><span data-stu-id="af968-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="af968-118">Lai novērstu turpmāku problēmu novēršanu, var būt nepieciešams sekot līdzi transporta atbalstam par SPF, DKIM un. vai DMARC kļūmēm.</span><span class="sxs-lookup"><span data-stu-id="af968-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>