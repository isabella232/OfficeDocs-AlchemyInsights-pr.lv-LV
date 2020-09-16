---
title: Fails ir atvērts kā tikai lasāms
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: 2fdb4f048c2bee022a49c2cca2ce9770f42a87a2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745597"
---
# <a name="file-open-read-only"></a><span data-ttu-id="1e751-102">Fails ir atvērts kā tikai lasāms</span><span class="sxs-lookup"><span data-stu-id="1e751-102">File open read-only</span></span>

<span data-ttu-id="1e751-103">Iespējams, ka, atverot failus, tie tiek atvērti kā tikai lasāmi.</span><span class="sxs-lookup"><span data-stu-id="1e751-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="1e751-104">Dažos gadījumos tas paredzēts papildu drošībai, piemēram, kad atverat failus no interneta, un citos laikos to var veikt, izmantojot iestatījumu, kas var tikt mainīts.</span><span class="sxs-lookup"><span data-stu-id="1e751-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="1e751-105">Tālāk ir norādīti daži scenāriji, kad fails tiek atvērts kā tikai lasāms, un dažas darbības, ko varat veikt, lai to mainītu.</span><span class="sxs-lookup"><span data-stu-id="1e751-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="1e751-106">**Mana antivīruss izraisa to atvēršanu tikai lasāmu**</span><span class="sxs-lookup"><span data-stu-id="1e751-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="1e751-107">Dažas pretvīrusu programmas var jūs pasargāt no potenciāli nedrošiem failiem, atverot tos tikai lasāmus.</span><span class="sxs-lookup"><span data-stu-id="1e751-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="1e751-108">Iespējams, jums būs jāsazinās ar savu pretvīrusu pakalpojumu sniedzēju, lai uzzinātu, kā pielāgot šos iestatījumus.</span><span class="sxs-lookup"><span data-stu-id="1e751-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="1e751-109">BitDefender, piemēram, ir saturs, kas tiek pievienots lietojumprogrammu izslēgšanas šeit: [kā pievienot lietojumprogrammu vai procesu izņēmumus BitDefender Control Center](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="1e751-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="1e751-110">**Vai faila rekvizīti ir iestatīti kā tikai lasāmi?**</span><span class="sxs-lookup"><span data-stu-id="1e751-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="1e751-111">Varat pārbaudīt faila rekvizītus, ar peles labo pogu noklikšķinot uz faila un izvēloties rekvizīti.</span><span class="sxs-lookup"><span data-stu-id="1e751-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="1e751-112">Ja ir atzīmēta izvēles rūtiņa tikai lasāms, varat to atlasīt un noklikšķināt uz Labi.</span><span class="sxs-lookup"><span data-stu-id="1e751-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="1e751-113">**Saturs ir aizsargātā skatā**</span><span class="sxs-lookup"><span data-stu-id="1e751-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="1e751-114">Faili no interneta un citām iespējami nedrošām vietām var saturēt vīrusus, tārpus vai cita veida ļaunprogrammatūru, kas var kaitēt jūsu datoram.</span><span class="sxs-lookup"><span data-stu-id="1e751-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="1e751-115">Tas parasti attiecas arī uz tiem e-pasta pielikumiem vai lejupielādētajiem failiem.</span><span class="sxs-lookup"><span data-stu-id="1e751-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="1e751-116">Lai aizsargātu datoru, faili no šīm potenciāli nedrošām atrašanās vietām tiek atvērti aizsargātā skatā.</span><span class="sxs-lookup"><span data-stu-id="1e751-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="1e751-117">Izmantojot aizsargātu skatu, varat lasīt failu un skatīt tā saturu, vienlaikus samazinot riskus.</span><span class="sxs-lookup"><span data-stu-id="1e751-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="1e751-118">Papildinformāciju par aizsargāto skatu un to, kā mainīt iestatījumus, skatiet šajā rakstā: [kas ir aizsargāts skats?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="1e751-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="1e751-119">**Vai OneDrive ir pilna?**</span><span class="sxs-lookup"><span data-stu-id="1e751-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="1e751-120">Ja fails ir saglabāts pakalpojumā OneDrive un jūsu OneDrive krātuves vieta ir pilna, jūs nevarēsit saglabāt dokumentu, kamēr nebūsit atvēlētajā vietā.</span><span class="sxs-lookup"><span data-stu-id="1e751-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="1e751-121">Varat pārbaudīt savu brīvo vietu pakalpojumā OneDrive, paziņojumu centrā noklikšķinot uz OneDrive ikonas un izvēloties pārvaldīt krātuvi, vai arī varat doties uz [https://onedrive.live.com](https://onedrive.live.com) , pierakstīties un atzīmēt izmantotās vietas apjomu ekrāna kreisajā apakšējā stūrī.</span><span class="sxs-lookup"><span data-stu-id="1e751-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="1e751-122">**Vai sistēma Office ir aktivizēta?**</span><span class="sxs-lookup"><span data-stu-id="1e751-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="1e751-123">Ja sistēma Office nav aktivizēta vai jūsu abonementa derīguma termiņš ir beidzies, iespējams, ka jums ir tikai lasīšanas režīma samazinātas funkcionalitātes režīms.</span><span class="sxs-lookup"><span data-stu-id="1e751-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="1e751-124">Informāciju par to, kā aktivizēt sistēmu Office, skatiet šeit: [nelicencēts produkts un aktivizācijas kļūdas sistēmā Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="1e751-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="1e751-125">**Ja viss pārējais nelīdz...**</span><span class="sxs-lookup"><span data-stu-id="1e751-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="1e751-126">Mēģiniet restartēt datoru</span><span class="sxs-lookup"><span data-stu-id="1e751-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="1e751-127">Office atjauninājumu instalēšana</span><span class="sxs-lookup"><span data-stu-id="1e751-127">Install Office updates</span></span>
    
- <span data-ttu-id="1e751-128">Office tiešsaistes labošanas veikšana</span><span class="sxs-lookup"><span data-stu-id="1e751-128">Perform an Online repair of Office</span></span>
    

