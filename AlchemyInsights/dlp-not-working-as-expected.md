---
title: DLP nedarbojas, kā paredzēts
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 1ea457bd69e7d545cf761a0be849695738b19d8b
ms.sourcegitcommit: d6ea6f4456a582559f27b34c0b9455a86a8e61f1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/31/2019
ms.locfileid: "35941075"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="67030-102">DLP nedarbojas, kā paredzēts</span><span class="sxs-lookup"><span data-stu-id="67030-102">DLP not working as expected</span></span>

<span data-ttu-id="67030-103">Vai jums ir problēmas ar **Datu zaudējumu novēršanas (DLP)** programmā Office 365 nedarbojas, kā paredzēts?</span><span class="sxs-lookup"><span data-stu-id="67030-103">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="67030-104">Šādā gadījumā pārliecinieties, vai jūsu **DLP politika** ir iestatīta pareizi un datos ir kādas **DLP politika** meklē, kad tas tiek vērtēts.</span><span class="sxs-lookup"><span data-stu-id="67030-104">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
 <span data-ttu-id="67030-105">**Ar ko izveido DLP**</span><span class="sxs-lookup"><span data-stu-id="67030-105">**Setting up DLP**</span></span>
  
<span data-ttu-id="67030-106">DLP politika ļauj identificēt un aizsargāt sensitīvu informāciju savā uzņēmumā.</span><span class="sxs-lookup"><span data-stu-id="67030-106">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="67030-107">Lai uzstādīšanas DLP politikai, izmantot informācijas [šeit](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="67030-107">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="67030-108">**DLP politiku meklējiet**</span><span class="sxs-lookup"><span data-stu-id="67030-108">**What DLP policies look for**</span></span>
  
<span data-ttu-id="67030-109">Lietojot **iebūvēto konfidenciālas informācijas tipiem** Office 365 drošības un saskaņotības centrs, DLP politiku izskatīsies noteiktiem rakstiem un elementu atklāšanu jutīgu šādas.</span><span class="sxs-lookup"><span data-stu-id="67030-109">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="67030-110">**Iebūvēts jutīgas informācijas veidus**</span><span class="sxs-lookup"><span data-stu-id="67030-110">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="67030-111">Par iebūvēto paaugstināta riska veidiem un kas DLP politika meklē, kad atklāt slepenu tipa informāciju meklējiet: [Meklēt kādus sensitīvu informāciju](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="67030-111">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="67030-112">**Pielāgota jutīga informācija veidus**</span><span class="sxs-lookup"><span data-stu-id="67030-112">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="67030-113">Ja jūs mēģināt izveidot pielāgotus jutīgas informācijas veidus, izmantot raksta informāciju, kā izveidot pielāgotu paaugstināta riska veids: [izveidot pielāgotu jutīgas informācijas tipu](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="67030-113">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="67030-114">**Testēt DLP politikas**</span><span class="sxs-lookup"><span data-stu-id="67030-114">**Test a DLP policy**</span></span>

<span data-ttu-id="67030-115">Pārbaudīt datus, izmantojot iebūvētos vai pielāgotos jutīgas informācijas veidu, izmantot **testa tipa** opcijai **klasifikācijas** > **jutīga informācija veidus**.</span><span class="sxs-lookup"><span data-stu-id="67030-115">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="67030-116">Papildinformāciju skatiet [testa pielāgota jutīga informācija veidus](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="67030-116">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="67030-117">**Ziņojumi**</span><span class="sxs-lookup"><span data-stu-id="67030-117">**Reports**</span></span>
  
- <span data-ttu-id="67030-118">Iegūtu precīzus datus atziņas ar [DLP ziņojumus.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="67030-118">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="67030-119">Sk. Īpašas sīkākas ziņas par notikumu ar [Negadījuma ziņojumu](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="67030-119">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
