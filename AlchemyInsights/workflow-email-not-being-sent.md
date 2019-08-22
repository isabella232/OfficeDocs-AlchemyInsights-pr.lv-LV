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
ms.openlocfilehash: 261fe1b1bc815dd4ad568051cfefad1e214b957e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530888"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="a3adf-102">Darbplūsmu, e-pasts netiek nosūtīts uz koplietošanas vides SharePoint sarakstā vai bibliotēkā</span><span class="sxs-lookup"><span data-stu-id="a3adf-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="a3adf-103">E-pastu no darbplūsmas netiek nosūtītas visiem lietotājiem vai tikai noteiktiem lietotājiem, vai jūs redzat kļūdu **, e-pasta ziņojumu nevar nosūtīt. Pārliecinieties, vai e-pasts ir derīgs adresāts**.</span><span class="sxs-lookup"><span data-stu-id="a3adf-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="a3adf-104">Pārbaudiet, ja lietotājs atrodas vietņu kolekcijas **Visi cilvēki** atļaujas grupai (lietotāju informācijas saraksts).</span><span class="sxs-lookup"><span data-stu-id="a3adf-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="a3adf-105">Parauga tiešai URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="a3adf-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="a3adf-106">Ja lietotājs neeksistē, pārliecinieties, vai lietotājs ir parakstīts uz lapu.</span><span class="sxs-lookup"><span data-stu-id="a3adf-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="a3adf-107">Ja tas ir ārējais lietotājs, pārliecinieties, ka savu ielūgumu pieņēma.</span><span class="sxs-lookup"><span data-stu-id="a3adf-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="a3adf-108">Ja lietotāju grupas atļaujas, pārliecinieties, vai e-pasta adrese ir pareiza.</span><span class="sxs-lookup"><span data-stu-id="a3adf-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="a3adf-109">Ja šeit nav iestatīti lietotāju e-pasta adresi, pēc tam izveidojiet brīdinājuma paraugu šī lietotāja, kas liek šī lietotāja konta sinhronizācijas no lietotāju profiliem, SharePoint šai vietņu kolekcijai.</span><span class="sxs-lookup"><span data-stu-id="a3adf-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="a3adf-110">E-pastu no darbplūsmas tiek nosūtīti vietņu kolekcijas administratorus, bet ne citiem lietotājiem un redzēt kļūdas **HTTP aizliegts uz <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span><span class="sxs-lookup"><span data-stu-id="a3adf-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="a3adf-111">Sk. [Liegta piekļuve, kad sūtāt e-pasta ziņojumu SharePoint grupai](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="a3adf-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="a3adf-112">Arī, pārliecinieties, vai **ierobežotu piekļuvi lietotāja atļauju slēgts režīmā** vietņu kolekcijas līdzekli nav aktīvs.</span><span class="sxs-lookup"><span data-stu-id="a3adf-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="a3adf-113">Saistītās tēmas</span><span class="sxs-lookup"><span data-stu-id="a3adf-113">Related topics</span></span>
<span data-ttu-id="a3adf-114">Vēlaties izmēģināt Microsoft SharePoint Online Flow?</span><span class="sxs-lookup"><span data-stu-id="a3adf-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="a3adf-115">Radīt plūsmu</span><span class="sxs-lookup"><span data-stu-id="a3adf-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="a3adf-116">SharePoint un plūsmas</span><span class="sxs-lookup"><span data-stu-id="a3adf-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


