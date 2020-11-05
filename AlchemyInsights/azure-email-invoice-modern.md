---
title: Modernā Azure e-pasta rēķini
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
- "9003801"
- "6866"
ms.openlocfilehash: 65df6091a97d4937379ded384a78b5d07aa76e42
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922065"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="00c2c-102">E-pasta rēķinu izrakstīšana Azure</span><span class="sxs-lookup"><span data-stu-id="00c2c-102">Email invoicing in Azure</span></span>

<span data-ttu-id="00c2c-103">Lai atjauninātu savas e-pasta rēķinu preferences, jums ir jābūt īpašniekam vai līdzstrādnieka lomai norēķinu profilā vai tā norēķinu kontā.</span><span class="sxs-lookup"><span data-stu-id="00c2c-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="00c2c-104">Kad būsit pieteicies, visi lietotāji, kuriem ir īpašnieks, līdzstrādnieks, lasītāji un rēķinu pārvaldnieka lomas norēķinu profilā, saņems rēķinu e-pasta ziņojumā.</span><span class="sxs-lookup"><span data-stu-id="00c2c-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="00c2c-105">Pierakstieties [Azure portālā](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="00c2c-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="00c2c-106">Meklējiet **izmaksu pārvaldību + norēķini**.</span><span class="sxs-lookup"><span data-stu-id="00c2c-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="00c2c-107">Atlasiet **rēķinus** no kreisās puses un pēc tam lapas augšdaļā atlasiet **e-pasta rēķins** .</span><span class="sxs-lookup"><span data-stu-id="00c2c-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="00c2c-108">Ja jums ir vairāki norēķinu profili, atlasiet norēķinu profilu un pēc tam atlasiet **pieteikties**.</span><span class="sxs-lookup"><span data-stu-id="00c2c-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="00c2c-109">Atlasiet **atjaunināt**.</span><span class="sxs-lookup"><span data-stu-id="00c2c-109">Select **Update**.</span></span>
6. <span data-ttu-id="00c2c-110">Ja jums ir vairāki norēķinu profili, atlasiet norēķinu profilu un pēc tam atlasiet **pieteikties**.</span><span class="sxs-lookup"><span data-stu-id="00c2c-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="00c2c-111">Jūs piešķirat citiem piekļuvi, lai skatītu, lejupielādētu un apmaksātu rēķinus, piešķirot tiem rēķinu pārvaldnieka lomu MCA vai MPA norēķinu profilam.</span><span class="sxs-lookup"><span data-stu-id="00c2c-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="00c2c-112">Ja esat pieteicies saņemt rēķinu e-pasta ziņojumā, lietotāji saņem arī rēķinus e-pasta ziņojumā.</span><span class="sxs-lookup"><span data-stu-id="00c2c-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="00c2c-113">Pierakstieties [Azure portālā](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="00c2c-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="00c2c-114">Meklējiet **izmaksu pārvaldību + norēķini**.</span><span class="sxs-lookup"><span data-stu-id="00c2c-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="00c2c-115">Atlasiet **norēķinu profilus** no kreisās puses.</span><span class="sxs-lookup"><span data-stu-id="00c2c-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="00c2c-116">Sarakstā norēķinu profili atlasiet norēķinu profilu, kuram vēlaties piešķirt rēķinu pārvaldnieka lomu.</span><span class="sxs-lookup"><span data-stu-id="00c2c-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="00c2c-117">Kreisās puses pusē atlasiet **piekļuves vadība (IAM)** un pēc tam lapas augšdaļā atlasiet **Pievienot** .</span><span class="sxs-lookup"><span data-stu-id="00c2c-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="00c2c-118">Nolaižamajā sarakstā lomai atlasiet **rēķinu pārvaldnieks**.</span><span class="sxs-lookup"><span data-stu-id="00c2c-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="00c2c-119">Ievadiet lietotāja e-pasta adresi, lai piešķirtu piekļuvi.</span><span class="sxs-lookup"><span data-stu-id="00c2c-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="00c2c-120">Atlasiet **Saglabāt** , lai piešķirtu lomu.</span><span class="sxs-lookup"><span data-stu-id="00c2c-120">Select **Save** to assign the role.</span></span>
