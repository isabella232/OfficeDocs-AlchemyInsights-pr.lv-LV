---
title: Problēma ar atribūtu un tvēruma filtru
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481894"
---
# <a name="problem-with-attribute-and-scoping-filter"></a><span data-ttu-id="c1eef-102">Problēma ar atribūtu un tvēruma filtru</span><span class="sxs-lookup"><span data-stu-id="c1eef-102">Problem with attribute and scoping filter</span></span>

<span data-ttu-id="c1eef-103">**Problēma ar konfliktējošām UPN vērtībām**</span><span class="sxs-lookup"><span data-stu-id="c1eef-103">**Issue with conflicting UPN values**</span></span>

<span data-ttu-id="c1eef-104">Darba diena līdz AD lietotājam, kas nodrošina funkciju WORKDAY uz reklāmu lietotāju nodrošinājums, rāda kļūdas ziņojuma **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span><span class="sxs-lookup"><span data-stu-id="c1eef-104">The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span></span> <span data-ttu-id="c1eef-105">Operācija neizdevās, jo UPN vērtība, kas ir nodrošināta pievienošana/modificēšana, nav unikāls meža mērogs.</span><span class="sxs-lookup"><span data-stu-id="c1eef-105">The operation failed because UPN value provided for addition/modification is not unique forest-wide.</span></span> <span data-ttu-id="c1eef-106">Detalizēta informācija par kļūdu: **CONSTRAINT_ATT_TYPE-userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="c1eef-106">Error Details: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span></span>

<span data-ttu-id="c1eef-107">**UserPrincipalName** vērtība, ko WORKDAY Connector mēģina iestatīt, veidojot ad lietotāja kontu, jau ir iekļauta Target ad domēnā.</span><span class="sxs-lookup"><span data-stu-id="c1eef-107">The **userPrincipalName** value that Workday connector is trying to set when creating the AD user account already exists in the target AD domain.</span></span> <span data-ttu-id="c1eef-108">Tas nozīmē, ka (1) lietotājs jau pastāv un atbilstošo ID pārbaude neizdevās lietotājam vai (2) UPN ģenerēšanas kārtula ģenerēja konfliktējošu vērtību.</span><span class="sxs-lookup"><span data-stu-id="c1eef-108">This implies that either (1) the user already exists and the matching ID check failed for the user or (2) the UPN generation rule generated a conflicting value.</span></span>

<span data-ttu-id="c1eef-109">Tālāk ir norādītas ieteicamās risinājuma darbības.</span><span class="sxs-lookup"><span data-stu-id="c1eef-109">Here are the suggested resolution steps:</span></span>

<span data-ttu-id="c1eef-110">Ja lietotājs jau pastāv un atbilstošo ID pārbaude neizdevās saistīt darba dienu kontu ar Active Directory kontu, pēc tam pārbaudiet, vai atbilstības ID atribūts (parasti **employeeID**) gan WORKDAY, gan ad ir precīza atbilstība.</span><span class="sxs-lookup"><span data-stu-id="c1eef-110">If the user already exists and the matching ID check failed to link the Workday account to Active Directory account, then check if the matching ID attribute (typically **employeeID**) in both Workday and AD have an exact match.</span></span> <span data-ttu-id="c1eef-111">Ja viņiem nav atbilstību, tas nozīmē, ka ir nepieciešams novērst datu problēmu.</span><span class="sxs-lookup"><span data-stu-id="c1eef-111">If they don't have a match, it is a data issue that needs to be fixed.</span></span> <span data-ttu-id="c1eef-112">Piemēram, ja EmployeeID darbdienā ir 001052 un REKLĀMā tas ir 1052, tad nodrošināšanas programmai neizdosies sasaistīt šos divus kontus un mēģinās izveidot lietotāju, kas jau pastāv.</span><span class="sxs-lookup"><span data-stu-id="c1eef-112">For example, if the EmployeeID in Workday is 001052 and in AD it is 1052, then the provisioning engine will fail to link the two accounts and will try to create a user that already exists.</span></span> <span data-ttu-id="c1eef-113">Šajā gadījumā risinājums ir mainīt **EmployeeID** vērtību reklāmā, lai iekļautu sākuma nulles, lai padarītu to 001052.</span><span class="sxs-lookup"><span data-stu-id="c1eef-113">The solution in this case is to change the **EmployeeID** value in AD to include the leading zeros to make it 001052.</span></span>
<span data-ttu-id="c1eef-114">Ja UPN ģenerētajā izteiksmē netiek ģenerēta unikāla vērtība, apsveriet iespēju izmantot funkciju **SelectUniqueValue** , lai katru reizi ģenerētu unikālu vērtību.</span><span class="sxs-lookup"><span data-stu-id="c1eef-114">If the UPN-generating expression is not generating a unique value, consider using the de-duplication function **SelectUniqueValue** to generate a unique value each time.</span></span>

<span data-ttu-id="c1eef-115">**Funkcija WORKDAY līdz AD lietotāja nodrošinājumam neiestata pārvaldnieka atribūta vērtību AD lietotāja kontam**</span><span class="sxs-lookup"><span data-stu-id="c1eef-115">**Workday to AD User Provisioning does not set manager attribute value for AD user account**</span></span>

<span data-ttu-id="c1eef-116">Funkcija WORKDAY uz AD lietotāju nodrošināšanas darbu neiestata **pārvaldnieka** atribūta vērtību ad lietotāju kontiem.</span><span class="sxs-lookup"><span data-stu-id="c1eef-116">The Workday to AD User Provisioning job is not setting the **manager** attribute value for AD user accounts.</span></span> <span data-ttu-id="c1eef-117">Ir iespējami divi scenāriji, kad šāda darbība ir redzama:</span><span class="sxs-lookup"><span data-stu-id="c1eef-117">There are two possible scenarios when this behavior is seen:</span></span>

1. <span data-ttu-id="c1eef-118">Vadītāju darba dienās nevar atrisināt atbilstošajā AD lietotāja kontā, jo nav šī pārvaldnieka tvēruma.</span><span class="sxs-lookup"><span data-stu-id="c1eef-118">The manager in Workday cannot be resolved to a corresponding AD User account because the manager is not in scope.</span></span>
2. <span data-ttu-id="c1eef-119">**Vairāku ad domains** scenārijs: vadītājs, kas ir WORKDAY, neatrodas tajā pašā domēnā, kur lietotājs.</span><span class="sxs-lookup"><span data-stu-id="c1eef-119">In a **multiple AD domains** scenario, the manager in Workday is not present in the same domain as the user.</span></span>

<span data-ttu-id="c1eef-120">Lai atrisinātu šo problēmu, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="c1eef-120">Try these steps to resolve the issue:</span></span>

1. <span data-ttu-id="c1eef-121">Ja esat definējis tvēruma filtrus, vispirms pārbaudiet, vai vadītājs ir tvērumā un vai tas atbilst klauzulai tvērums.</span><span class="sxs-lookup"><span data-stu-id="c1eef-121">If you have defined scoping filters, first check if the manager is in scope and that it satisfies the scoping clause.</span></span> <span data-ttu-id="c1eef-122">Ja vadītājs neapmierina tvēruma filtru, mainiet filtru tā, lai vadītājs būtu arī nodrošināšanas darbības sfērā.</span><span class="sxs-lookup"><span data-stu-id="c1eef-122">If the manager does not satisfy the scoping filter, change the filter so that the manager is also in scope of the provisioning operation.</span></span>
2. <span data-ttu-id="c1eef-123">Ja jums ir vairāki AD domēni, savienotāja ir zināms ierobežojums nespējai atrisināt starpdomēnu pārvaldnieka atsauces.</span><span class="sxs-lookup"><span data-stu-id="c1eef-123">If you have multiple AD domains, then the connector has a known limitation of inability to resolve cross-domain manager references.</span></span>

<span data-ttu-id="c1eef-124">Lai iegūtu papildinformāciju par to, kā konfigurēt darba dienu automatizētai konfigurēšanai, skatiet rakstu [apmācība: darbdienas konfigurēšana automātiskai lietotāju nodrošināšanai](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="c1eef-124">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>













