---
title: Darbplūsmas e-pasts netiek sūtīts
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748996"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="c6479-102">Darbplūsmas e-pasts netiek sūtīts SharePoint sarakstam vai bibliotēkai</span><span class="sxs-lookup"><span data-stu-id="c6479-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="c6479-103">E-pasta ziņojumi no darbplūsmām netiek nosūtīti visiem lietotājiem vai tikai konkrētiem lietotājiem, vai arī redzat kļūdas ziņojumu, **ka e-pasta ziņojums nav nosūtīts. Pārliecinieties, vai e-pasta ziņojumam ir derīgs adresāts**.</span><span class="sxs-lookup"><span data-stu-id="c6479-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="c6479-104">Pārbaudiet, vai lietotājs ir šīs vietņu kolekcijas grupā **visas personas** atļaujas (lietotāju informācijas saraksts).</span><span class="sxs-lookup"><span data-stu-id="c6479-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="c6479-105">Izlases tiešā vietrāža URL: https:// <tenant> . SharePoint.com/sites/ <sitename> /_layouts/15/People.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="c6479-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="c6479-106">Ja lietotājs nepastāv, pārliecinieties, vai lietotājs ir pierakstījies lapā.</span><span class="sxs-lookup"><span data-stu-id="c6479-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="c6479-107">Ja tas ir ārējs lietotājs, pārliecinieties, vai viņa uzaicinājums ir apstiprināts.</span><span class="sxs-lookup"><span data-stu-id="c6479-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="c6479-108">Ja lietotājs pastāv atļauju grupā, pārliecinieties, vai e-pasta adrese ir pareiza.</span><span class="sxs-lookup"><span data-stu-id="c6479-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="c6479-109">Ja lietotāju e-pasta adrese šeit nav iestatīta, pēc tam izveidojiet brīdinājuma paraugu šim lietotājam, kas veic šī lietotāja konta sinhronizāciju no SharePoint lietotāju profiliem šajā vietņu kolekcijā.</span><span class="sxs-lookup"><span data-stu-id="c6479-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="c6479-110">E-pasta ziņojumi no darbplūsmām tiek nosūtīti vietņu kolekcijas administratoriem, bet ne citiem lietotājiem, un tiek rādīts kļūdas ziņojums, **kas aizliegts <span>https:</span>//URL/_vti_bin/Client.xvc.SP.Utilities.Utility.SendEmail**.</span><span class="sxs-lookup"><span data-stu-id="c6479-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="c6479-111">Skatiet rakstu [piekļuve liegta, ja nosūtāt e-pasta ziņojumu SharePoint grupai](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="c6479-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="c6479-112">Pārliecinieties arī, vai ir aktivizēts neaktīvs **lietotāju atļauju bloķēšanas režīms** .</span><span class="sxs-lookup"><span data-stu-id="c6479-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="c6479-113">Saistītās tēmas</span><span class="sxs-lookup"><span data-stu-id="c6479-113">Related topics</span></span>
<span data-ttu-id="c6479-114">Vai vēlaties izmēģināt Microsoft plūsmu pakalpojumā SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="c6479-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="c6479-115">Izveidot plūsmu</span><span class="sxs-lookup"><span data-stu-id="c6479-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="c6479-116">SharePoint un plūsma</span><span class="sxs-lookup"><span data-stu-id="c6479-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


