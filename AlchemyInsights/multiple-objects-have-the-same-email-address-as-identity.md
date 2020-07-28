---
title: Vairākiem objektiem ir viena e-pasta adrese kā identitāte
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439191"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="7037b-102">Vairākiem objektiem ir viena e-pasta adrese kā identitāte</span><span class="sxs-lookup"><span data-stu-id="7037b-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="7037b-103">**Vairāki objekti**</span><span class="sxs-lookup"><span data-stu-id="7037b-103">**Multiple objects**</span></span>

<span data-ttu-id="7037b-104">Viens no biežākajiem šīs kļūdas iemesliem ir tas, ka ar to pašu e-pasta adresi nav iespējams pareizi maršrutēt Outlook Web Access pieprasījumu vairāku objektu klātbūtnē.</span><span class="sxs-lookup"><span data-stu-id="7037b-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="7037b-105">Lai atrastu šos objektus, izpildiet tālāk norādītās komandas.</span><span class="sxs-lookup"><span data-stu-id="7037b-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="7037b-106">· Iegūt adresātu<email address></span><span class="sxs-lookup"><span data-stu-id="7037b-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="7037b-107">· Iegūt lietotāju<email address></span><span class="sxs-lookup"><span data-stu-id="7037b-107">· Get-User <email address></span></span>

<span data-ttu-id="7037b-108">· Get-user <email address> -SoftDeletedUser</span><span class="sxs-lookup"><span data-stu-id="7037b-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="7037b-109">· Saņemt kontaktpersonas<email address></span><span class="sxs-lookup"><span data-stu-id="7037b-109">· Get-Contact <email address></span></span>

<span data-ttu-id="7037b-110">· Get-Pastkaste <email address> — PublicFolder</span><span class="sxs-lookup"><span data-stu-id="7037b-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="7037b-111">· Get-Pastkaste <email address> — IncludeSoftDeletedMailbox</span><span class="sxs-lookup"><span data-stu-id="7037b-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="7037b-112">· Get-Pastkaste <email address> — InactiveMailboxOnly</span><span class="sxs-lookup"><span data-stu-id="7037b-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="7037b-113">Lai atrisinātu šo problēmu, noņemiet vairākus objektus ar tādu pašu e-pasta identitāti un pārliecinieties, vai ir viens objekts ar konkrētu e-pasta identitāti un tā adresāta tips ir UserMailbox.</span><span class="sxs-lookup"><span data-stu-id="7037b-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="7037b-114">**To pašu adresi izmanto biznesa un patērētāju pastkastēm**</span><span class="sxs-lookup"><span data-stu-id="7037b-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="7037b-115">Vēl viens iemesls ir, kad to pašu adresi izmanto uzņēmumu un patērētāju pastkastēm.</span><span class="sxs-lookup"><span data-stu-id="7037b-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="7037b-116">Šajā gadījumā lietotājam ir jāmaina primārais patērētāju aizstājvārds, līdz kafejnīca atbalsta šo scenāriju.</span><span class="sxs-lookup"><span data-stu-id="7037b-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="7037b-117">Šī ir pastāvīga kļūda, kas nepazūd bez iejaukšanās.</span><span class="sxs-lookup"><span data-stu-id="7037b-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="7037b-118">Detalizētu informāciju skatiet rakstā [e-pasta adreses vai tālruņa numura maiņa savam Microsoft kontam](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span><span class="sxs-lookup"><span data-stu-id="7037b-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>