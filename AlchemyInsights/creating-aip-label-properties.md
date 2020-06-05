---
title: AIP etiķešu politikas izveide
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: de7d76564cabb0a5dd1a836984df6b1a63b2b218
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569205"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="ea89d-102">AIP etiķešu politikas izveide</span><span class="sxs-lookup"><span data-stu-id="ea89d-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="ea89d-103">Azure informācijas aizsardzības (AIP) etiķetes var izmantot ar pilnu datu klāstu, ko organizācija parasti izveido un uzglabā no zemākās personas datu klasifikācijas līdz visaugstākajai ļoti konfidenciālo datu klasifikācijai.</span><span class="sxs-lookup"><span data-stu-id="ea89d-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="ea89d-104">Azure informācijas aizsardzības politikas attiecas uz Azure informācijas aizsardzība (AIP) Classic klients, nevis [AIP vienotais marķēšanas klients](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="ea89d-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="ea89d-105">AIP politikā var konfigurēt vairākus elementus, tostarp opcijas, piemēram:</span><span class="sxs-lookup"><span data-stu-id="ea89d-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="ea89d-106">Opcija, kurai etiķete ļaus administratoriem vai lietotājam klasificēt un aizsargāt (neobligāti) dokumentus un e-pastus</span><span class="sxs-lookup"><span data-stu-id="ea89d-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="ea89d-107">Opciju, lai ieviestu klasifikāciju, kad lietotāji saglabā dokumentus un sūta e-pastu</span><span class="sxs-lookup"><span data-stu-id="ea89d-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="ea89d-108">Iespēja automātiski marķēt e-pasta ziņojumu, pamatojoties uz tā pielikumiem.</span><span class="sxs-lookup"><span data-stu-id="ea89d-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="ea89d-109">Opciju, lai kontrolētu, vai informācijas aizsardzības josla tiek parādīta Office lietojumprogrammās</span><span class="sxs-lookup"><span data-stu-id="ea89d-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="ea89d-110">Papildu opcijas un informāciju par Azure informācijas aizsardzības politiku, skatiet: [pārskats par Azure informācijas aizsardzības politika](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="ea89d-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="ea89d-111">Citiem noderīgiem resursiem par AIP politikām skatiet:</span><span class="sxs-lookup"><span data-stu-id="ea89d-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="ea89d-112">Pamācība: konfigurējiet Azure informācijas aizsardzības politikas iestatījumus un izveidojiet jaunu etiķeti</span><span class="sxs-lookup"><span data-stu-id="ea89d-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="ea89d-113">Azure informācijas aizsardzības politikas konfigurēšana</span><span class="sxs-lookup"><span data-stu-id="ea89d-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="ea89d-114">Veidojiet un konfigurējiet jutīguma etiķetes un to politikas</span><span class="sxs-lookup"><span data-stu-id="ea89d-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="ea89d-115">Norādījumi par vispārējiem scenārijiem, kas izmanto Azure informācijas aizsardzību</span><span class="sxs-lookup"><span data-stu-id="ea89d-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="ea89d-116">Azure informācijas aizsardzības dokumentācijas pārskatīšana</span><span class="sxs-lookup"><span data-stu-id="ea89d-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="ea89d-117">Prasības Azure informācijas aizsardzība</span><span class="sxs-lookup"><span data-stu-id="ea89d-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="ea89d-118">Ātri sākt apmācība Azure informācijas aizsardzība</span><span class="sxs-lookup"><span data-stu-id="ea89d-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="ea89d-119">Lejupielādēt Azure informācijas aizsardzības klients</span><span class="sxs-lookup"><span data-stu-id="ea89d-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)