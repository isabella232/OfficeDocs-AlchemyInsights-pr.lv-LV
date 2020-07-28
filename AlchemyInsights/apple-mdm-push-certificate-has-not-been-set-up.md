---
title: Apple MDM push sertifikāts nav iestatīts
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439380"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="bcc6e-102">Apple MDM push sertifikāts nav iestatīts</span><span class="sxs-lookup"><span data-stu-id="bcc6e-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="bcc6e-103">Apple MDM push sertifikāts (zināms arī kā Apple push Notification Service (APN) sertifikāts) nav konfigurēts jūsu abonementam.</span><span class="sxs-lookup"><span data-stu-id="bcc6e-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="bcc6e-104">Ja nav konfigurēts Apple MDM push sertifikāts, jūs nevarat reģistrēties un pārvaldīt iOS un Mac OS ierīces.</span><span class="sxs-lookup"><span data-stu-id="bcc6e-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="bcc6e-105">Pēc sertifikāta pievienošanas Intune lietotāji var instalēt uzņēmuma portāla lietojumprogrammu, lai reģistrētu savas iOS ierīces.</span><span class="sxs-lookup"><span data-stu-id="bcc6e-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="bcc6e-106">Atlasiet **"es piekrītu".**</span><span class="sxs-lookup"><span data-stu-id="bcc6e-106">Select **"I agree."**</span></span> <span data-ttu-id="bcc6e-107">lai piešķirtu Microsoft atļauju nosūtīt datus Apple.</span><span class="sxs-lookup"><span data-stu-id="bcc6e-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="bcc6e-108">Atlasiet **lejupielādēt USA** Intune sertifikāta parakstīšanas pieprasījumu, kas nepieciešams, lai izveidotu Apple MDM push sertifikātu.</span><span class="sxs-lookup"><span data-stu-id="bcc6e-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="bcc6e-109">Fails tiek izmantots, lai pieprasītu uzticamības relācijas sertifikātu no Apple push sertifikātu portāla.</span><span class="sxs-lookup"><span data-stu-id="bcc6e-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="bcc6e-110">Atlasiet **izveidot savu MDM push sertifikātu** , lai pārietu uz Apple push Certificates portālu.</span><span class="sxs-lookup"><span data-stu-id="bcc6e-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="bcc6e-111">Pierakstieties ar sava uzņēmuma Apple ID un pēc tam atlasiet **izveidot sertifikātu**.</span><span class="sxs-lookup"><span data-stu-id="bcc6e-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="bcc6e-112">Atlasiet **izvēlēties failu**, pārlūkojiet līdz sertifikāta parakstīšanas pieprasījuma failam un pēc tam izvēlieties **augšupielādēt**.</span><span class="sxs-lookup"><span data-stu-id="bcc6e-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="bcc6e-113">Apstiprinājuma lapā izvēlieties **lejupielādēt** , lai lejupielādētu sertifikātu (. pem) failu, un saglabājiet failu lokāli.</span><span class="sxs-lookup"><span data-stu-id="bcc6e-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="bcc6e-114">**Piezīme**: sertifikāts ir saistīts ar Apple ID, kas tiek izmantots, lai to izveidotu.</span><span class="sxs-lookup"><span data-stu-id="bcc6e-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="bcc6e-115">Kā paraugpraksi izmantojiet uzņēmuma Apple ID pārvaldības uzdevumiem un pārliecinieties, vai pastkasti pārrauga vairākas personas vai izmantojot adresātu sarakstu.</span><span class="sxs-lookup"><span data-stu-id="bcc6e-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="bcc6e-116">Nekad neizmantojiet personisku Apple ID.</span><span class="sxs-lookup"><span data-stu-id="bcc6e-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="bcc6e-117">Izmantojiet to pašu Apple ID, lai atjaunotu Apple push sertifikātu ik pēc 12 mēnešiem.</span><span class="sxs-lookup"><span data-stu-id="bcc6e-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="bcc6e-118">Ievadiet Apple ID, ko izmantojāt, lai izveidotu savu Apple MDM push sertifikātu.</span><span class="sxs-lookup"><span data-stu-id="bcc6e-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="bcc6e-119">Ierakstiet šo ID kā atgādinājumu, kad ir jāatjauno sertifikāts.</span><span class="sxs-lookup"><span data-stu-id="bcc6e-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="bcc6e-120">Dodieties uz sertifikātu (. pem) failu, izvēlieties **Atvērt**un pēc tam izvēlieties **augšupielādēt**.</span><span class="sxs-lookup"><span data-stu-id="bcc6e-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="bcc6e-121">Izmantojot pašpiegādes sertifikātu, Intune var reģistrēt un pārvaldīt Apple ierīces.</span><span class="sxs-lookup"><span data-stu-id="bcc6e-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>