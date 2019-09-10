---
title: Failu atvērt kā tikai lasāmu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: eddd427b159a782abf53adda934de8b15a02ed00
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822241"
---
# <a name="file-open-read-only"></a><span data-ttu-id="82f24-102">Failu atvērt kā tikai lasāmu</span><span class="sxs-lookup"><span data-stu-id="82f24-102">File open read-only</span></span>

<span data-ttu-id="82f24-103">Jūs varat konstatēt, ka, atverot failus, tie tiek atvērti kā tikai lasāmi.</span><span class="sxs-lookup"><span data-stu-id="82f24-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="82f24-104">Dažos gadījumos tas ir papildu drošībai, piemēram, atverot failus no interneta un citos laikos, tas var būt saistīts ar iestatījumu, ko var mainīt.</span><span class="sxs-lookup"><span data-stu-id="82f24-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="82f24-105">Lūk, daži scenāriji, kuros fails tiek atvērts kā tikai lasāms, un dažas darbības, ko varat veikt, lai to mainītu.</span><span class="sxs-lookup"><span data-stu-id="82f24-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="82f24-106">**Mans antivīruss rada viņiem atvērt tikai lasāmu**</span><span class="sxs-lookup"><span data-stu-id="82f24-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="82f24-107">Dažas pretvīrusu programmas var aizsargāt no potenciāli nedrošiem failiem, atverot tos kā tikai lasāmus.</span><span class="sxs-lookup"><span data-stu-id="82f24-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="82f24-108">Lai uzzinātu, kā pielāgot šos iestatījumus, iespējams, ir jāpārbauda pretvīrusu programmatūras nodrošinātājs.</span><span class="sxs-lookup"><span data-stu-id="82f24-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="82f24-109">BitDefender, piemēram, ir saturs, pievienojot pieteikumu izņēmumi šeit: [kā pievienot pieteikumu vai procesu izslēgšanu BitDefender Control Center](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="82f24-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="82f24-110">**Vai faila rekvizīti ir iestatīti kā tikai lasāmi?**</span><span class="sxs-lookup"><span data-stu-id="82f24-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="82f24-111">Jūs varat pārbaudīt faila rekvizītus, ar peles labo pogu noklikšķinot uz faila un izvēloties Properties.</span><span class="sxs-lookup"><span data-stu-id="82f24-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="82f24-112">Ja tikai lasāms atribūts ir atzīmēts, varat noņemt atzīmi un noklikšķiniet uz Labi.</span><span class="sxs-lookup"><span data-stu-id="82f24-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="82f24-113">**Saturs ir aizsargātajā skatā**</span><span class="sxs-lookup"><span data-stu-id="82f24-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="82f24-114">Faili no interneta un no citām potenciāli nedrošām atrašanās vietām var saturēt vīrusus, tārpus vai cita veida ļaunprogrammatūru, kas var kaitēt jūsu datoram.</span><span class="sxs-lookup"><span data-stu-id="82f24-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="82f24-115">Parasti tas attiecas arī uz lejupielādētajiem e-pasta pielikumiem vai failiem.</span><span class="sxs-lookup"><span data-stu-id="82f24-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="82f24-116">Lai palīdzētu aizsargāt datoru, faili no šīm potenciāli nedrošām atrašanās vietām tiek atvērti aizsargātajā skatā.</span><span class="sxs-lookup"><span data-stu-id="82f24-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="82f24-117">Izmantojot aizsargāto skatu, varat lasīt failu un redzēt tā saturu, vienlaikus samazinot riskus.</span><span class="sxs-lookup"><span data-stu-id="82f24-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="82f24-118">Lai iegūtu papildinformāciju par aizsargāto skatu un kā mainīt iestatījumus, skatiet šo rakstu: [kas ir aizsargāts skats?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="82f24-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="82f24-119">**Vai OneDrive ir pilna?**</span><span class="sxs-lookup"><span data-stu-id="82f24-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="82f24-120">Ja fails ir saglabāts pakalpojumā OneDrive un jūsu OneDrive krātuves vieta ir pilna, dokumentu nevarēs saglabāt, kamēr neesat atvēlētajā vietā.</span><span class="sxs-lookup"><span data-stu-id="82f24-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="82f24-121">Varat pārbaudīt savu brīvo vietu pakalpojumā OneDrive, paziņojumu centrā noklikšķinot uz ikonas OneDrive un izvēloties pārvaldīt krātuvi, vai varat doties uz [http://onedrive.live.com](http://onedrive.live.com), pierakstīties un atzīmēt izmantotās telpas apjomu ekrāna apakšējā kreisajā malā.</span><span class="sxs-lookup"><span data-stu-id="82f24-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [http://onedrive.live.com](http://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="82f24-122">**Vai Office ir aktivizēta?**</span><span class="sxs-lookup"><span data-stu-id="82f24-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="82f24-123">Ja Office nav aktivizēts vai abonementa derīguma termiņš ir beidzies, varat būt tikai lasāms samazinātas funkcionalitātes režīmā.</span><span class="sxs-lookup"><span data-stu-id="82f24-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="82f24-124">Informāciju par Office aktivizēšanu skatiet šeit: [nelicencēta produkta un Office aktivizācijas kļūdas](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="82f24-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="82f24-125">**Ja visi cits neizdodas...**</span><span class="sxs-lookup"><span data-stu-id="82f24-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="82f24-126">Mēģiniet restartēt datoru</span><span class="sxs-lookup"><span data-stu-id="82f24-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="82f24-127">Office atjauninājumu instalēšana</span><span class="sxs-lookup"><span data-stu-id="82f24-127">Install Office updates</span></span>
    
- <span data-ttu-id="82f24-128">Veikt Office tiešsaistes labošanu</span><span class="sxs-lookup"><span data-stu-id="82f24-128">Perform an Online repair of Office</span></span>
    

