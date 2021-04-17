---
title: Azure rēķini pa e-pastu
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
- "9003801"
- "6866"
ms.openlocfilehash: 4df8c49880fe638c1659f76edc0905532d091e45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820833"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="b47d5-102">Azure e-pasta rēķini</span><span class="sxs-lookup"><span data-stu-id="b47d5-102">Email invoicing in Azure</span></span>

<span data-ttu-id="b47d5-103">Lai mainītu e-pasta adresi rēķinu saņemšanai jums ir jābūt norēķinu profila vai norēķinu konta īpašniekam vai līdzstrādniekam.</span><span class="sxs-lookup"><span data-stu-id="b47d5-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="b47d5-104">Pēc reģistrācijas, visi lietotāji ar īpašnieka, līdzstrādnieka, lasītāja un rēķinu pārvaldnieka lomām norēķinu profilā saņems rēķinu savā e-pastā.</span><span class="sxs-lookup"><span data-stu-id="b47d5-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="b47d5-105">Pierakstieties [Azure portālā](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="b47d5-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="b47d5-106">Meklējiet **Izmaksu pārvaldība + norēķini**.</span><span class="sxs-lookup"><span data-stu-id="b47d5-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="b47d5-107">Atlasiet **Rēķini** kreisajā pusē un pēc tam atlasiet **Rēķins e-pastā** lapas augšdaļā.</span><span class="sxs-lookup"><span data-stu-id="b47d5-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="b47d5-108">Ja jums ir vairāki norēķini profili, atlasiet vienu un pēc tam atlasiet **Reģistrēt**.</span><span class="sxs-lookup"><span data-stu-id="b47d5-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="b47d5-109">Atlasiet **Atjaunināt**.</span><span class="sxs-lookup"><span data-stu-id="b47d5-109">Select **Update**.</span></span>
6. <span data-ttu-id="b47d5-110">Ja jums ir vairāki norēķini profili, atlasiet vienu un pēc tam atlasiet **Reģistrēt**.</span><span class="sxs-lookup"><span data-stu-id="b47d5-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="b47d5-111">Piešķirat lietotājam rēķinu pārvaldnieka lomu MCA vai MPA norēķinu profilā, jūs piešķirat lietotājam piekļuvi skatīt, lejupielādēt un apmaksāt rēķinus.</span><span class="sxs-lookup"><span data-stu-id="b47d5-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="b47d5-112">Ja izvēlējāties saņemt rēķinu e-pastā, tas tiks nosūtīts arī uz citu lietotāju e-pastiem.</span><span class="sxs-lookup"><span data-stu-id="b47d5-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="b47d5-113">Pierakstieties [Azure portālā](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="b47d5-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="b47d5-114">Meklējiet **Izmaksu pārvaldība + norēķini**.</span><span class="sxs-lookup"><span data-stu-id="b47d5-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="b47d5-115">Atlasiet **Norēķinu profili** kreisajā pusē.</span><span class="sxs-lookup"><span data-stu-id="b47d5-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="b47d5-116">Norēķinu profilu sarakstā atlasiet norēķinu profilu, kuram vēlaties piešķirt rēķinu pārvaldnieka lomu.</span><span class="sxs-lookup"><span data-stu-id="b47d5-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="b47d5-117">Atlasiet **Piekļuves vadība (IAM)** kreisajā pusē un pēc tam atlasiet **Pievienot** lapas augšdaļā.</span><span class="sxs-lookup"><span data-stu-id="b47d5-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="b47d5-118">Lomu nolaižamajā sarakstā atlasiet **Rēķinu pārvaldnieks**.</span><span class="sxs-lookup"><span data-stu-id="b47d5-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="b47d5-119">Ievadiet lietotāja e-pasta adresi, lai piešķirtu piekļuvi.</span><span class="sxs-lookup"><span data-stu-id="b47d5-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="b47d5-120">Atlasiet **Saglabāt**, lai piešķirtu lomu.</span><span class="sxs-lookup"><span data-stu-id="b47d5-120">Select **Save** to assign the role.</span></span>
