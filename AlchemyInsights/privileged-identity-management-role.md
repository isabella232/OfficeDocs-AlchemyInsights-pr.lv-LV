---
title: Priviliģētā identitātes pārvaldības loma
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088880"
---
# <a name="privileged-identity-managementpim-role"></a><span data-ttu-id="0b130-102">Priviliģētā identitātes pārvaldības (PIM) loma</span><span class="sxs-lookup"><span data-stu-id="0b130-102">Privileged Identity Management(PIM) role</span></span>

<span data-ttu-id="0b130-103">**Pēc lomas aktivizēšanas atļaujas nav piešķirtas**</span><span class="sxs-lookup"><span data-stu-id="0b130-103">**Permissions are not granted after activating a role**</span></span>

<span data-ttu-id="0b130-104">Aktivizējot lomu Azure AD priviliģētā identitātes pārvaldībā (PIM), aktivizēšana var netikt uzreiz izplatīta visiem portāliem, kuriem nepieciešama privileģētā loma.</span><span class="sxs-lookup"><span data-stu-id="0b130-104">When you activate a role in Azure AD Privileged Identity Management (PIM), the activation may not instantly propagate to all portals that require the privileged role.</span></span> <span data-ttu-id="0b130-105">Dažreiz pat tad, ja izmaiņas tiek izplatītas, tīmekļa kešatmiņa portālā var izraisīt izmaiņas, kas uzreiz neietekmēs.</span><span class="sxs-lookup"><span data-stu-id="0b130-105">Sometimes, even if the change is propagated, web caching in a portal may result in the change not taking effect immediately.</span></span>

<span data-ttu-id="0b130-106">Ja aktivizācija ir aizkavēta, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="0b130-106">If your activation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="0b130-107">Izrakstieties no Azure portāla un pēc tam atkal pierakstieties.</span><span class="sxs-lookup"><span data-stu-id="0b130-107">Sign out of the Azure portal and then sign back in.</span></span> <span data-ttu-id="0b130-108">Aktivizējot Azure AD lomu vai Azure resursa lomu, redzēsit aktivizēšanas posmus.</span><span class="sxs-lookup"><span data-stu-id="0b130-108">When you activate an Azure AD role or an Azure resource role, you will see the stages of your activation.</span></span> <span data-ttu-id="0b130-109">Kad visi posmi ir pabeigti, tiks parādīta saite Izrakstīties.</span><span class="sxs-lookup"><span data-stu-id="0b130-109">Once all the stages are complete, you will see a 'Sign out' link.</span></span> <span data-ttu-id="0b130-110">Varat izmantot šo saiti, lai izrakstītos. Tas atrisinās lielāko daļu gadījumu aktivizēšanas atlikšanai.</span><span class="sxs-lookup"><span data-stu-id="0b130-110">You can use this link to sign out. This will solve most cases for activation delay.</span></span>
2. <span data-ttu-id="0b130-111">Programmā PIM pārbaudiet, vai esat norādīts kā lomas dalībnieks.</span><span class="sxs-lookup"><span data-stu-id="0b130-111">In PIM, verify that you are listed as the member of the role.</span></span>
3. <span data-ttu-id="0b130-112">Ja aktivizējat Exchange administratora lomu, noteikti izrakstieties un pierakstieties vēlreiz.</span><span class="sxs-lookup"><span data-stu-id="0b130-112">If you are activating the Exchange Administrator role, make sure you sign out and sign back in.</span></span> <span data-ttu-id="0b130-113">Ja problēma joprojām pastāv, atveriet atbalsta biļeti un uzlabojiet to kā problēmu.</span><span class="sxs-lookup"><span data-stu-id="0b130-113">If the problem persists, open a support ticket and raise this as an issue.</span></span> <span data-ttu-id="0b130-114">Ja izmantojat Exchange administratora lomu, lai piekļūtu drošības un atbilstības centram, skatiet nākamo darbību.</span><span class="sxs-lookup"><span data-stu-id="0b130-114">If you are using your Exchange Administrator role to access the Security and Compliance Center, see the next step.</span></span>
4. <span data-ttu-id="0b130-115">Ja aktivizējat lomu, lai piekļūtu drošības un atbilstības centram, vai, ja aktivizējat SharePoint administratora lomu, jums būs zināma aktivizēšanas aizkave no dažām minūtēm līdz pat dažām stundām.</span><span class="sxs-lookup"><span data-stu-id="0b130-115">If you are activating a role to access the Security and Compliance Center or if you are activating the SharePoint Administrator role, you will experience some activation delay from a few minutes up to a few hours.</span></span> <span data-ttu-id="0b130-116">Šī ir zināma problēma, un mēs aktīvi strādājam ar šīm grupām, lai atrisinātu šo problēmu pēc iespējas ātrāk.</span><span class="sxs-lookup"><span data-stu-id="0b130-116">This is a known issue and we are actively working with these teams to resolve this issue as soon as possible.</span></span>

<span data-ttu-id="0b130-117">Papildinformāciju skatiet rakstā:</span><span class="sxs-lookup"><span data-stu-id="0b130-117">For more information, see:</span></span>

- [<span data-ttu-id="0b130-118">Azure AD lomu aktivizēšana PIM</span><span class="sxs-lookup"><span data-stu-id="0b130-118">Activate my Azure AD roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [<span data-ttu-id="0b130-119">Azure resursu lomu aktivizēšana PIM</span><span class="sxs-lookup"><span data-stu-id="0b130-119">Activate my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

<span data-ttu-id="0b130-120">**Atļaujas netiek noņemtas pēc lomas deaktivizēšanas vai lomas aktivizēšanas derīguma termiņa beigām**</span><span class="sxs-lookup"><span data-stu-id="0b130-120">**Permissions are not removed after deactivating a role or the role activation expires**</span></span>

<span data-ttu-id="0b130-121">Deaktivizējot lomu Azure AD privileģētā identitātes pārvaldībā vai pēc tam, kad beidzas lomas aktivizēšanas perioda termiņš, iespējams, ir aizkave, kur jums joprojām ir piekļuve.</span><span class="sxs-lookup"><span data-stu-id="0b130-121">When you deactivate a role in Azure AD Privileged Identity Management or when a role activation period expires, there might be a delay where you continue to have access.</span></span>

<span data-ttu-id="0b130-122">Ja deaktivizēšana ir aizkavēta, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="0b130-122">If your deactivation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="0b130-123">Ja aktivizējat Exchange administratora lomu vai lomas aktivizēšanas perioda beigas, un jūs nodarbina nozīmīgu atlikšanu pirms atļauju noņemšanas, atveriet atbalsta biļeti un informējiet savu atbalsta inženieri par to, lai palīdzētu jums iesniegt biļeti ar privileģētu piekļuves pārvaldības (PAM) grupu sistēmā Office par šo problēmu.</span><span class="sxs-lookup"><span data-stu-id="0b130-123">If you are deactivating the Exchange Administrator role or the role activation period expires, and you notice a significant delay before the permissions are removed, open a support ticket and tell your support engineer to help you file a ticket with the Privileged Access Management (PAM) team inside Office about this issue.</span></span>
2. <span data-ttu-id="0b130-124">Ja aktivizēšanas periodam ir beidzies derīgums, bet joprojām ir atvērta pārlūka sesija, slēdziet pārlūkprogrammu.</span><span class="sxs-lookup"><span data-stu-id="0b130-124">If the activation period has expired, but you still have the browser session open, close your browser.</span></span> <span data-ttu-id="0b130-125">Jūs varat turpināt izmantot šo lomu, līdz aizvērsit šo sesiju.</span><span class="sxs-lookup"><span data-stu-id="0b130-125">You can continue to use the role until you close that session.</span></span> <span data-ttu-id="0b130-126">Šī ir zināma problēma, un mēs raugāmies uz iespējamu labojumu, lai aktīvi atsauktu katru sesiju, kad aktivizācija ir beigusies.</span><span class="sxs-lookup"><span data-stu-id="0b130-126">This is a known issue and we are looking at a potential fix to actively revoke each session once activation has expired.</span></span>

<span data-ttu-id="0b130-127">Ja kavējums ir atšķirīgs no šiem diviem scenārijiem, lūdzu, atveriet atbalsta biļeti.</span><span class="sxs-lookup"><span data-stu-id="0b130-127">If your delay is different than these two scenarios, please open a support ticket.</span></span>
