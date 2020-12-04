---
title: Papildu autentifikācijas principi, kas attiecas uz Microsoft Edge
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
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573523"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="d688a-102">Papildu autentifikācijas principi, kas attiecas uz Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="d688a-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="d688a-103">Tālāk ir norādīti papildu autentifikācijas jēdzieni, kas attiecas uz Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="d688a-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="d688a-104">**Proaktīvā autentifikācija**</span><span class="sxs-lookup"><span data-stu-id="d688a-104">**Proactive Authentication**</span></span>

<span data-ttu-id="d688a-105">Iespējojot [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) politiku, Microsoft Edge mēģinās proaktīvi autentificēt lietotājus, izmantojot Microsoft pakalpojumus.</span><span class="sxs-lookup"><span data-stu-id="d688a-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="d688a-106">Regulāros intervālos tā izmantos tiešsaistes pakalpojumu, lai pārbaudītu, vai ir atjaunināts saraksts, kurā ir iekļauta konfigurācija, kas reglamentē proaktīvo autentifikāciju.</span><span class="sxs-lookup"><span data-stu-id="d688a-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="d688a-107">Priekšrocības: proaktīvā autentifikācija nodrošina autentifikāciju ar galvenajiem pakalpojumiem, piemēram, Office jaunās cilnes lapu.</span><span class="sxs-lookup"><span data-stu-id="d688a-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="d688a-108">Turklāt, ja Bing tiek izmantots kā meklēšanas dzinējs, proaktīvā autentifikācija uzlabo adrešu joslas veiktspēju un palīdz ģenerēt meklēšanas rezultātus, kas ir personalizēti uzņēmuma vajadzībām.</span><span class="sxs-lookup"><span data-stu-id="d688a-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="d688a-109">**Windows Hello CredUI NTLM autentifikācijai**</span><span class="sxs-lookup"><span data-stu-id="d688a-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="d688a-110">Ja vienotā pierakstīšanās (SSO) nav pieejama, ja tīmekļa vietne mēģina lietotājam pierakstīties, izmantojot NTLM vai sarunas mehānismu, šis līdzeklis ļaus lietotājam kopīgot OS akreditācijas datus ar tīmekļa vietni un izpildīt autentifikācijas problēmu, izmantojot Windows Hello Cred UI.</span><span class="sxs-lookup"><span data-stu-id="d688a-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="d688a-111">Šī pierakstīšanās plūsma būs pieejama tikai operētājsistēmā Windows 10 un tikai tiem lietotājiem, kas nesaņem SSO NTLM vai sarunas laikā.</span><span class="sxs-lookup"><span data-stu-id="d688a-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="d688a-112">**Saglabāto paroļu izmantošana, lai automātiski pierakstītos**</span><span class="sxs-lookup"><span data-stu-id="d688a-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="d688a-113">Lietotāji, kas saglabā paroles pārlūkprogrammā Microsoft Edge, var iespējot automātisko pierakstīšanos tīmekļa vietnēm, kurās ir saglabāti akreditācijas dati.</span><span class="sxs-lookup"><span data-stu-id="d688a-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="d688a-114">Lietotāji var ieslēgt vai izslēgt šo līdzekli pakalpojumā edge://settings/passwords, un varat to konfigurēt [paroļu pārvaldnieka](https://go.microsoft.com/fwlink/?linkid=2134622) politikās.</span><span class="sxs-lookup"><span data-stu-id="d688a-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
