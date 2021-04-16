---
title: Fails ir atvērts kā tikai lasāms
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: e478572ea82e5ea11bac9fd7eacafb833253235d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813191"
---
# <a name="file-open-read-only"></a><span data-ttu-id="0cf2c-102">Fails ir atvērts kā tikai lasāms</span><span class="sxs-lookup"><span data-stu-id="0cf2c-102">File open read-only</span></span>

<span data-ttu-id="0cf2c-103">Iespējams, ka, atverot failus, tie tiek atvērti kā tikai lasāmi.</span><span class="sxs-lookup"><span data-stu-id="0cf2c-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="0cf2c-104">Dažos gadījumos tas notiek papildu drošības dēļ, piemēram, ja atverat failu no interneta, bet citos gadījumos to var izraisīt iestatījums, kuru var mainīt.</span><span class="sxs-lookup"><span data-stu-id="0cf2c-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="0cf2c-105">Lūk, daži scenāriji, kad fails tiek atvērts tikai lasāms, un dažas darbības, kas jāveic, lai to mainītu.</span><span class="sxs-lookup"><span data-stu-id="0cf2c-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="0cf2c-106">**Manas pretvīrusu aizsardzības dēļ šīs programmas tiek atvērtas kā tikai lasāmas**</span><span class="sxs-lookup"><span data-stu-id="0cf2c-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="0cf2c-107">Dažas pretvīrusu programmas var aizsargāt no potenciāli nedrošiem failiem, atverot tos kā tikai lasāmus.</span><span class="sxs-lookup"><span data-stu-id="0cf2c-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="0cf2c-108">Iespējams, jums būs jāzinās pie sava pretvīrusu aizsardzības pakalpojumu sniedzēja, lai uzzinātu, kā pielāgot šos iestatījumus.</span><span class="sxs-lookup"><span data-stu-id="0cf2c-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="0cf2c-109">Piemēram, BitDefender ir informācija par lietojumprogrammu izņēmumu pievienošanu šeit: Kā pievienot lietojumprogrammu vai [procesu izņēmumus Bitdefender vadības centrā](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="0cf2c-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="0cf2c-110">**Vai faila rekvizīti ir iestatīti, lai faili būtu tikai lasāmi?**</span><span class="sxs-lookup"><span data-stu-id="0cf2c-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="0cf2c-111">Varat pārbaudīt faila rekvizītus, ar peles labo pogu noklikšķinot uz faila un izvēloties Rekvizīti.</span><span class="sxs-lookup"><span data-stu-id="0cf2c-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="0cf2c-112">Ja ir atzīmēts atribūts Tikai lasāms, varat noņemiet atzīmi un noklikšķināt uz Labi.</span><span class="sxs-lookup"><span data-stu-id="0cf2c-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="0cf2c-113">**Saturs ir aizsargātā skatā**</span><span class="sxs-lookup"><span data-stu-id="0cf2c-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="0cf2c-114">Failos no interneta un citām iespējami nedrošām atrašanās vietām var būt vīrusi, tārpi vai cita veida ļaunprogrammatūra, kas var kaitēt datoram.</span><span class="sxs-lookup"><span data-stu-id="0cf2c-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="0cf2c-115">Tas parasti attiecas arī uz e-pasta pielikumiem un lejupielādētiem failiem.</span><span class="sxs-lookup"><span data-stu-id="0cf2c-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="0cf2c-116">Lai aizsargātu datoru, faili no šīm iespējami nedrošajām atrašanās vietām tiek atvērti aizsargātajā skatā.</span><span class="sxs-lookup"><span data-stu-id="0cf2c-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="0cf2c-117">Izmantojot aizsargāto skatu, var lasīt failu un skatīt tā saturu, vienlaikus samazinot riskus.</span><span class="sxs-lookup"><span data-stu-id="0cf2c-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="0cf2c-118">Papildinformāciju par aizsargāto skatu un iestatījumu maiņu skatiet šajā rakstā: [Kas ir aizsargāts skats?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="0cf2c-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="0cf2c-119">**Vai OneDrive krātuve ir pilna?**</span><span class="sxs-lookup"><span data-stu-id="0cf2c-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="0cf2c-120">Ja fails tiek glabāts pakalpojumā OneDrive un OneDrive krātuve ir pilna, dokumentu nevar saglabāt, kamēr nav atbrīvota krātuves vieta.</span><span class="sxs-lookup"><span data-stu-id="0cf2c-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="0cf2c-121">Varat pārbaudīt brīvo vietu pakalpojumā OneDrive, noklikšķinot uz OneDrive ikonas paziņojumu centrā un izvēloties Pārvaldīt krātuvi, vai arī varat doties uz , pierakstīties un skatīt izmantotās vietas daudzumu ekrāna apakšējā kreisajā [https://onedrive.live.com](https://onedrive.live.com) stūrī.</span><span class="sxs-lookup"><span data-stu-id="0cf2c-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="0cf2c-122">**Vai sistēma Office ir aktivizēta?**</span><span class="sxs-lookup"><span data-stu-id="0cf2c-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="0cf2c-123">Ja Office nav aktivizēta vai jūsu abonementa derīguma termiņš ir beidzies, iespējams, ir aktivizēts samazinātas funkcionalitātes režīms ar tikai lasīšanas iespējām.</span><span class="sxs-lookup"><span data-stu-id="0cf2c-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="0cf2c-124">Informāciju par Office aktivizēšanu skatiet rakstā: [Nelicencēts produkts un aktivizācijas kļūdas sistēmā Office.](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)</span><span class="sxs-lookup"><span data-stu-id="0cf2c-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="0cf2c-125">**Ja neizdodas nekas cits...**</span><span class="sxs-lookup"><span data-stu-id="0cf2c-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="0cf2c-126">Mēģiniet restartēt datoru</span><span class="sxs-lookup"><span data-stu-id="0cf2c-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="0cf2c-127">Office atjauninājumu instalēšana</span><span class="sxs-lookup"><span data-stu-id="0cf2c-127">Install Office updates</span></span>
    
- <span data-ttu-id="0cf2c-128">Veiciet Office tiešsaistes labošanu</span><span class="sxs-lookup"><span data-stu-id="0cf2c-128">Perform an Online repair of Office</span></span>
    

