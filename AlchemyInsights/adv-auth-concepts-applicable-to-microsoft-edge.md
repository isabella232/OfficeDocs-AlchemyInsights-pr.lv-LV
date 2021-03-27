---
title: Paplašinātie autentifikācijas jēdzieni, kas attiecas uz Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398592"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="11f4a-102">Paplašinātie autentifikācijas jēdzieni, kas attiecas uz Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="11f4a-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="11f4a-103">Tālāk ir papildu autentifikācijas jēdzieni, kas attiecas uz Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="11f4a-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="11f4a-104">**Proactive Authentication**</span><span class="sxs-lookup"><span data-stu-id="11f4a-104">**Proactive Authentication**</span></span>

<span data-ttu-id="11f4a-105">Ja iespējojat [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) politiku, Microsoft Edge mēģina proaktīvi autentificēt pierakstītos lietotājus, izmantojot Microsoft pakalpojumus.</span><span class="sxs-lookup"><span data-stu-id="11f4a-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="11f4a-106">Regulāros intervālos tas izmantos tiešsaistes pakalpojumu, lai meklētu atjauninātu manifestu, kas ietver konfigurāciju, kas nosaka proaktīvu autentifikāciju.</span><span class="sxs-lookup"><span data-stu-id="11f4a-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="11f4a-107">Priekšrocības. Proaktīvā autentifikācija iespējo autentifikāciju atslēgas pakalpojumiem, piemēram, Office jaunas cilnes lapai.</span><span class="sxs-lookup"><span data-stu-id="11f4a-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="11f4a-108">Turklāt, ja Bing tiek izmantota kā meklētājprogramma, proaktīvā autentifikācija uzlabo adrešu joslas veiktspēju un palīdz ģenerēt meklēšanas rezultātus, kas pielāgoti jūsu uzņēmuma vajadzībām.</span><span class="sxs-lookup"><span data-stu-id="11f4a-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="11f4a-109">**Windows Hello CredUI NTLM autentifikācijai**</span><span class="sxs-lookup"><span data-stu-id="11f4a-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="11f4a-110">Ja vienotā pierakstīšanās (single sign-on — SSO) nav pieejama, tīmekļa vietne mēģina pierakstīties lietotājam, izmantojot NTLM vai apspriedēm mehānismu, šis līdzeklis sniedz lietotājam iespēju koplietot operētājsistēmas akreditācijas datus ar tīmekļa vietni un izpildīt autentifikācijas uzdevumu, izmantojot Windows Hello akreditācijas datu lietotāja interfeisu.</span><span class="sxs-lookup"><span data-stu-id="11f4a-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="11f4a-111">Šī pierakstīšanās plūsma tiks rādīta tikai sistēmā Windows 10 un tikai tiem lietotājiem, kuri nesaņem SSO NTLM vai apspriedīs uzdevumu.</span><span class="sxs-lookup"><span data-stu-id="11f4a-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="11f4a-112">**Saglabāto paroļu izmantošana, lai pierakstītos automātiski**</span><span class="sxs-lookup"><span data-stu-id="11f4a-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="11f4a-113">Lietotāji, kas saglabā paroles programmā Microsoft Edge, var iespējot automātisko pierakstīšanu tīmekļa vietnēs, kurās viņi ir saglabājis akreditācijas datus.</span><span class="sxs-lookup"><span data-stu-id="11f4a-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="11f4a-114">Lietotāji var ieslēgt vai izslēgt šo līdzekli edge://settings/passwords un varat to konfigurēt paroļu [pārvaldnieka politikās.](https://go.microsoft.com/fwlink/?linkid=2134622)</span><span class="sxs-lookup"><span data-stu-id="11f4a-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
