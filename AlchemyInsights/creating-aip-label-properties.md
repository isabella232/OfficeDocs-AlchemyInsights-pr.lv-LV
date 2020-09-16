---
title: ARA uzlīmju politikas izveide
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: bef170d8e38dcc91094b95604aeb1968d5c57fca
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732182"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="64870-102">ARA uzlīmju politikas izveide</span><span class="sxs-lookup"><span data-stu-id="64870-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="64870-103">Azure Information Protection (ARA) etiķetes var izmantot kopā ar visu datu diapazonu, ko organizācija parasti izveido un uzglabā no zemākās personas datu klasifikācijas līdz augstākai ļoti konfidenciālu datu klasifikācijai.</span><span class="sxs-lookup"><span data-stu-id="64870-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="64870-104">Azure informācijas aizsardzības politikas attiecas uz Azure Information Protection (AIP) klasisko klientu, nevis  [ARA unificētās marķēšanas klientu](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="64870-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="64870-105">ARA politikā varat konfigurēt vairākus elementus, tostarp opcijas, piemēram:</span><span class="sxs-lookup"><span data-stu-id="64870-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="64870-106">Opcijas, kuras etiķete ļaus administratoriem vai lietotāju klasificēšanai un aizsardzībai (neobligāti) dokumentus un e-pasta ziņojumus</span><span class="sxs-lookup"><span data-stu-id="64870-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="64870-107">Opcija ieviest klasifikāciju, ja lietotāji saglabā dokumentus un nosūta e-pastu</span><span class="sxs-lookup"><span data-stu-id="64870-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="64870-108">Opcija automātiski iezīmēt e-pasta ziņojumu, ņemot vērā tā pielikumus.</span><span class="sxs-lookup"><span data-stu-id="64870-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="64870-109">Opcija, lai kontrolētu, vai Office lietojumprogrammās tiek rādīta informācijas aizsardzības josla</span><span class="sxs-lookup"><span data-stu-id="64870-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="64870-110">Papildu opcijas un informāciju par Azure informācijas aizsardzības politikām skatiet šeit: [Azure informācijas aizsardzības politikas pārskats](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="64870-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="64870-111">Citus noderīgus resursus attiecībā uz AIP politikām skatiet:</span><span class="sxs-lookup"><span data-stu-id="64870-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="64870-112">Apmācība: Azure informācijas aizsardzības politikas iestatījumu konfigurēšana un jaunas etiķetes izveide</span><span class="sxs-lookup"><span data-stu-id="64870-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="64870-113">Azure informācijas aizsardzības politikas konfigurēšana</span><span class="sxs-lookup"><span data-stu-id="64870-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="64870-114">Jutīguma etiķešu un to politiku izveide un konfigurēšana</span><span class="sxs-lookup"><span data-stu-id="64870-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="64870-115">Padomi bieži lietotajiem scenārijiem, kuros tiek izmantota Azure informācijas aizsardzība</span><span class="sxs-lookup"><span data-stu-id="64870-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="64870-116">Azure informācijas aizsardzības dokumentācijas pārskatīšana</span><span class="sxs-lookup"><span data-stu-id="64870-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="64870-117">Azure informācijas aizsardzības prasības</span><span class="sxs-lookup"><span data-stu-id="64870-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="64870-118">Īsā lietošanas pamācība Azure informācijas aizsardzībai</span><span class="sxs-lookup"><span data-stu-id="64870-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="64870-119">Azure informācijas aizsardzības klienta lejupielāde</span><span class="sxs-lookup"><span data-stu-id="64870-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)