---
title: Problēmu novēršana saistībā ar notikumiem no e-pasta
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
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834846"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="46091-102">Problēmu novēršana saistībā ar notikumiem no e-pasta</span><span class="sxs-lookup"><span data-stu-id="46091-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="46091-103">Pārbaude, vai pastkastei šis līdzeklis ir iespējots: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span><span class="sxs-lookup"><span data-stu-id="46091-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="46091-104">Pēc tam skatiet žurnālus "Notikumi no **e-pasta" Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="46091-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="46091-105">Žurnālos "Notikumi no e-pasta" atrodiet InternetMessageId, kas atbilst vienumam pastkastē.</span><span class="sxs-lookup"><span data-stu-id="46091-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="46091-106">TrustScore nosaka, vai vienums ir pievienots vai nē.</span><span class="sxs-lookup"><span data-stu-id="46091-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="46091-107">Notikumi tiks pievienoti tikai tad, ja TrustScore = "Trusted".</span><span class="sxs-lookup"><span data-stu-id="46091-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="46091-108">TrustScore nosaka rekvizīti SPF, Dkim vai Dmarc, kuri ir ziņojuma iesākumā.</span><span class="sxs-lookup"><span data-stu-id="46091-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="46091-109">Lai skatītu šos rekvizītus:</span><span class="sxs-lookup"><span data-stu-id="46091-109">To view these properties:</span></span>

<span data-ttu-id="46091-110">**Outlook datora versija**</span><span class="sxs-lookup"><span data-stu-id="46091-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="46091-111">Atvērt vienumu</span><span class="sxs-lookup"><span data-stu-id="46091-111">Open the item</span></span>
- <span data-ttu-id="46091-112">File -> Properties -> Internet Headers</span><span class="sxs-lookup"><span data-stu-id="46091-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="46091-113">vai</span><span class="sxs-lookup"><span data-stu-id="46091-113">or</span></span>

<span data-ttu-id="46091-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="46091-114">**MFCMapi**</span></span>

- <span data-ttu-id="46091-115">Naviģēt uz vienumu iesūtnē</span><span class="sxs-lookup"><span data-stu-id="46091-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="46091-116">Meklējiet PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="46091-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="46091-117">Šie rekvizīti tiek noteikti un ierakstīti transporta un maršrutēšanas laikā.</span><span class="sxs-lookup"><span data-stu-id="46091-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="46091-118">Lai novērstu citas problēmas, iespējams, būs jāseko transporta atbalsta dienestam par kļūmēm SPF, DKIM un.vai DMARC.</span><span class="sxs-lookup"><span data-stu-id="46091-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>