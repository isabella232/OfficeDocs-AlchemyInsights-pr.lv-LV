---
title: Darbplūsmas e-pasts netiek sūtīts
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 391d3a2dcc2676a405065115f375c802d2492119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766140"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="72566-102">Darbplūsmas e-pasta netiek nosūtīts SharePoint saraksta vai bibliotēkas</span><span class="sxs-lookup"><span data-stu-id="72566-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="72566-103">E-pasta ziņojumi no darbplūsmas netiek sūtīti visiem lietotājiem vai tikai konkrētiem lietotājiem, vai arī tiek parādīts kļūdas ziņojums **nevar nosūtīt e-pasta ziņojumu. Pārliecinieties, vai e-pastam ir derīgs adresāts**.</span><span class="sxs-lookup"><span data-stu-id="72566-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="72566-104">Pārbaudiet, vai lietotājs ir vietņu kolekcijas **visas personas** atļaujas grupas (lietotāja informācijas saraksts).</span><span class="sxs-lookup"><span data-stu-id="72566-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="72566-105">Paraugs Direct URL: https://<tenant>. sharepoint.com/sites/<sitename>/_layouts/15/People.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="72566-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="72566-106">Ja lietotājs neeksistē, pārliecinieties, vai lietotājs ir pierakstījies lapā.</span><span class="sxs-lookup"><span data-stu-id="72566-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="72566-107">Ja tas ir ārējais lietotājs, pārliecinieties, vai viņu uzaicinājums ir akceptēts.</span><span class="sxs-lookup"><span data-stu-id="72566-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="72566-108">Ja lietotājs pastāv atļauju grupas, pārliecinieties, vai e-pasta adrese ir pareiza.</span><span class="sxs-lookup"><span data-stu-id="72566-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="72566-109">Ja lietotājiem e-pasta adrese nav iestatīta šeit, pēc tam izveidojiet parauga brīdinājumu šim lietotājam, kas liek sinhronizēt šo lietotāja kontu no SharePoint lietotāju profiliem šajā vietņu kolekcijā.</span><span class="sxs-lookup"><span data-stu-id="72566-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="72566-110">E-pasta ziņojumu no darbplūsmas tiek nosūtīti vietņu kolekcijas administratoriem, bet ne citiem lietotājiem un skatiet kļūdas **http aizliegts <span>https:</span>//URL/_vti_bin/Client.xvc.SP.Utilities.Utility.SendEmail**.</span><span class="sxs-lookup"><span data-stu-id="72566-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="72566-111">[Ja nosūtāt e-pasta ziņojumu SharePoint grupai](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups), skatiet sadaļu piekļuve liegta.</span><span class="sxs-lookup"><span data-stu-id="72566-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="72566-112">Arī pārliecināties, ka **ierobežotas piekļuves lietotāja atļaujas noslēgšanas režīmā** vietņu kolekcijas līdzeklis nav aktīvs.</span><span class="sxs-lookup"><span data-stu-id="72566-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="72566-113">Saistītās tēmas</span><span class="sxs-lookup"><span data-stu-id="72566-113">Related topics</span></span>
<span data-ttu-id="72566-114">Vai vēlaties izmēģināt Microsoft Flow pakalpojumā SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="72566-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="72566-115">Izveidot plūsmu</span><span class="sxs-lookup"><span data-stu-id="72566-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="72566-116">SharePoint un plūsmas</span><span class="sxs-lookup"><span data-stu-id="72566-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


