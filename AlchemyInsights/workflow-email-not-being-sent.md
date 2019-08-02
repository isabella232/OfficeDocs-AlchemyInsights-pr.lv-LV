---
title: Darbplūsmu, e-pasts netiek nosūtīts
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 783bf0a5721aa5db7088432c71e06cac6dc90513
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059610"
---
# <a name="workflow-email-is-not-being-sent"></a><span data-ttu-id="e1c2e-102">Darbplūsmu, e-pasts netiek nosūtīts</span><span class="sxs-lookup"><span data-stu-id="e1c2e-102">Workflow email is not being sent</span></span>

1. <span data-ttu-id="e1c2e-103">E-pastu no darbplūsmas netiek nosūtītas visiem lietotājiem vai tikai noteiktiem lietotājiem, vai jūs redzat kļūdu **, e-pasta ziņojumu nevar nosūtīt. Pārliecinieties, vai e-pasts ir derīgs adresāts**.</span><span class="sxs-lookup"><span data-stu-id="e1c2e-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

<span data-ttu-id="e1c2e-104">Pārbaudiet, ja lietotājs atrodas vietņu kolekcijas **Visi cilvēki** atļaujas grupai (lietotāju informācijas saraksts).</span><span class="sxs-lookup"><span data-stu-id="e1c2e-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="e1c2e-105">Parauga tiešai URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="e1c2e-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

- <span data-ttu-id="e1c2e-106">Ja lietotājs neeksistē, pārliecinieties, vai lietotājs ir parakstīts uz lapu.</span><span class="sxs-lookup"><span data-stu-id="e1c2e-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
- <span data-ttu-id="e1c2e-107">Ja tas ir ārējais lietotājs, pārliecinieties, ka savu ielūgumu pieņēma.</span><span class="sxs-lookup"><span data-stu-id="e1c2e-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
- <span data-ttu-id="e1c2e-108">Ja lietotāju grupas atļaujas, pārliecinieties, vai e-pasta adrese ir pareiza.</span><span class="sxs-lookup"><span data-stu-id="e1c2e-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
- <span data-ttu-id="e1c2e-109">Ja šeit nav iestatīti lietotāju e-pasta adresi, pēc tam izveidojiet brīdinājuma paraugu šī lietotāja, kas liek šī lietotāja konta sinhronizācijas no lietotāju profiliem, SharePoint šai vietņu kolekcijai.</span><span class="sxs-lookup"><span data-stu-id="e1c2e-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="e1c2e-110">E-pastu no darbplūsmas tiek nosūtīti vietņu kolekcijas administratorus, bet ne citiem lietotājiem un redzēt kļūdas \*\*HTTP aizliegts uz <spam> <spam> \*\* <spam> <spam>.</span><span class="sxs-lookup"><span data-stu-id="e1c2e-110">Email from Workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <spam><spam>https://URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**<spam><spam>.</span></span>
 

<span data-ttu-id="e1c2e-111">Sk. [Liegta piekļuve, kad nosūtītie e-pasta grupas](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="e1c2e-111">See [Access Denied when sent email to groups](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span></span>

<span data-ttu-id="e1c2e-112">Arī, pārliecinieties, vai **ierobežotu piekļuvi lietotāja atļauju slēgts režīmā** vietņu kolekcijas līdzekli nav aktīvs.</span><span class="sxs-lookup"><span data-stu-id="e1c2e-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>

## <a name="related-topics"></a><span data-ttu-id="e1c2e-113">Saistītās tēmas</span><span class="sxs-lookup"><span data-stu-id="e1c2e-113">Related topics</span></span>
- [<span data-ttu-id="e1c2e-114">Radīt plūsmu</span><span class="sxs-lookup"><span data-stu-id="e1c2e-114">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="e1c2e-115">SharePoint un plūsmas</span><span class="sxs-lookup"><span data-stu-id="e1c2e-115">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


