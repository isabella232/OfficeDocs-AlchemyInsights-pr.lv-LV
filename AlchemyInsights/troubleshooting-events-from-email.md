---
title: Problēmu novēršanas notikumi no e-pasta
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
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658741"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="f6943-102">Problēmu novēršanas notikumi no e-pasta</span><span class="sxs-lookup"><span data-stu-id="f6943-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="f6943-103">Pārbaudiet, vai pastkastei ir iespējots līdzeklis: \*\*Get-EventsFromEmailConfiguration-Identity <mailbox> \*\*</span><span class="sxs-lookup"><span data-stu-id="f6943-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="f6943-104">Pēc tam aplūkojiet notikumus no e-pasta žurnāliem **, eksportējot-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="f6943-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="f6943-105">Žurnālos "notikumi no e-pasta" atrodiet InternetMessageId, kas atbilst pastkastes elementam.</span><span class="sxs-lookup"><span data-stu-id="f6943-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="f6943-106">TrustScore nosaka, vai vienums ir pievienots.</span><span class="sxs-lookup"><span data-stu-id="f6943-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="f6943-107">Notikumi tiks pievienoti tikai tad, ja TrustScore = "uzticams".</span><span class="sxs-lookup"><span data-stu-id="f6943-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="f6943-108">TrustScore nosaka SPF, DKIM vai Dmarc rekvizīti, kas atrodas ziņojuma iesākumā.</span><span class="sxs-lookup"><span data-stu-id="f6943-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="f6943-109">Lai skatītu šos rekvizītus:</span><span class="sxs-lookup"><span data-stu-id="f6943-109">To view these properties:</span></span>

<span data-ttu-id="f6943-110">**Darbvirsmas Outlook**</span><span class="sxs-lookup"><span data-stu-id="f6943-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="f6943-111">Atvērt vienumu</span><span class="sxs-lookup"><span data-stu-id="f6943-111">Open the item</span></span>
- <span data-ttu-id="f6943-112">Failu-> rekvizīti — > interneta galvenes</span><span class="sxs-lookup"><span data-stu-id="f6943-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="f6943-113">vai</span><span class="sxs-lookup"><span data-stu-id="f6943-113">or</span></span>

<span data-ttu-id="f6943-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="f6943-114">**MFCMapi**</span></span>

- <span data-ttu-id="f6943-115">Pārvietošanās uz vienumu iesūtnē</span><span class="sxs-lookup"><span data-stu-id="f6943-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="f6943-116">PR_TRANSPORT_MESSAGE_HEADERS_W meklēšana</span><span class="sxs-lookup"><span data-stu-id="f6943-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="f6943-117">Šos rekvizītus nosaka un reģistrē transportēšanas un maršrutēšanas laikā.</span><span class="sxs-lookup"><span data-stu-id="f6943-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="f6943-118">Lai veiktu citas darbības problēmu novēršanai, iespējams, jums būs jāseko transporta atbalstam attiecībā uz SPF, DKIM un DMARC.</span><span class="sxs-lookup"><span data-stu-id="f6943-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>