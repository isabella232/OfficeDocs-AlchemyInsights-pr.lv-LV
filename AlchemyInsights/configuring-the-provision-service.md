---
title: Pakalpojumu sniedzēja konfigurēšana
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482871"
---
# <a name="configuring-the-provision-service"></a><span data-ttu-id="10287-102">Pakalpojumu sniedzēja konfigurēšana</span><span class="sxs-lookup"><span data-stu-id="10287-102">Configuring the Provision service</span></span>

<span data-ttu-id="10287-103">Lai veiktu automātisku lietotāja nodrošināšanu darbam, Azure AD ir nepieciešami derīgie akreditācijas dati, kas ļauj izveidot savienojumu ar darbadienu tīmekļa pakalpojumu API.</span><span class="sxs-lookup"><span data-stu-id="10287-103">For automated user provisioning to work, Azure AD requires valid credentials that allow it to connect to Workday Web Services API.</span></span> <span data-ttu-id="10287-104">Tālāk poga testa savienojums, kas pieejama sadaļā WORKDAY to AD User nodrošināšanas programma, validē arī, ja tā var izveidot savienojumu ar Azure AD Connect nodrošināšanas aģentu, kas saistīts ar reklāmas domēnu.</span><span class="sxs-lookup"><span data-stu-id="10287-104">Further, the Test Connection button on the Workday to AD User Provisioning app also validates if it is able to connect to the Azure AD Connect Provisioning Agent associated with the AD Domain.</span></span>

<span data-ttu-id="10287-105">Ja Azure portāls atgriež kļūdu, saglabājot akreditācijas datus, rīkojieties šādi:</span><span class="sxs-lookup"><span data-stu-id="10287-105">If the Azure portal is returning an error upon saving the credentials, follow the recommended steps below:</span></span>

1. <span data-ttu-id="10287-106">Apstipriniet, ka esat konfigurējis darba dienu integrācijas sistēmas lietotāja kontu, kā norādīts sadaļā apmācība [konfigurējiet integrācijas sistēmas lietotāju darbdienas](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)ietvaros.</span><span class="sxs-lookup"><span data-stu-id="10287-106">Confirm that you have configured Workday Integration System User account as stated in the tutorial section [Configure integration system user in Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
2. <span data-ttu-id="10287-107">Pārliecinieties, vai Azure AD Connect nodrošināšanas aģenta pakalpojums darbojas jūsu lokālajā Windows serverī, izmantojot pakalpojumu pārvaldības konsoli.</span><span class="sxs-lookup"><span data-stu-id="10287-107">Confirm that the Azure AD Connect Provisioning Agent Service is up and running on your on-premises Windows server using the Services Management Console.</span></span> <span data-ttu-id="10287-108">Varat arī pārbaudīt aģenta statusu Azure portālā, noklikšķinot uz pogas Skatīt lokālos aģentus.</span><span class="sxs-lookup"><span data-stu-id="10287-108">You can also check the status of the agent in the Azure portal by clicking the View on-premises agents button.</span></span>
3. <span data-ttu-id="10287-109">Pārliecinieties, vai ievadāt lauka "WORKDAY username" vērtību, izmantojot formātu username@workday nomnieka vārdu.</span><span class="sxs-lookup"><span data-stu-id="10287-109">Ensure that you are entering the value for "Workday Username" field using the format username@workday-tenant-name.</span></span> <span data-ttu-id="10287-110">Ja nav ievadīts darbdienas nomnieka vārds, darba dienu autentifikācija neizdevās.</span><span class="sxs-lookup"><span data-stu-id="10287-110">If the workday-tenant-name is missing, Workday authentication fails.</span></span>
4. <span data-ttu-id="10287-111">Ja konfigurējat integrāciju ar WORKDAY implementēšanas nomnieku, ņemiet vērā sava darba dienu nomnieka plānotās dīkstāves stundas.</span><span class="sxs-lookup"><span data-stu-id="10287-111">If you are configuring the integration with Workday implementation tenant, note the scheduled downtime hours of your Workday tenant.</span></span> <span data-ttu-id="10287-112">Funkcija WORKDAY ir ieplānojusi noteiktu laiku tās implementēšanai uz nedēļas nogales (parasti no piektdienas vakara līdz sestdienas rītam) un savienojamības kļūmes šajā dīkstāves logā ir zināma problēma, kas automātiski tiek novērsta, tiklīdz ieviešanas nomnieki atkal ir tiešsaistē.</span><span class="sxs-lookup"><span data-stu-id="10287-112">Workday has scheduled down time for its implementation tenants over weekends (usually from Friday evening to Saturday morning) and connectivity failures during this downtime window is a known issue that auto-resolves as soon as the implementation tenants are back online.</span></span>
5. <span data-ttu-id="10287-113">Retos gadījumos, iespējams, redzēsit šo kļūdu, ja ir mainīta integrācijas sistēmas lietotāja parole, jo nomnieka atsvaidzināšana vai konts ir bloķēts vai beidzies derīguma termiņš.</span><span class="sxs-lookup"><span data-stu-id="10287-113">In rare cases, you may also see this error if the password of the Integration System User changed due to tenant refresh or if the account is in locked or expired state.</span></span> <span data-ttu-id="10287-114">Lūdzu, pārbaudiet integrācijas sistēmas lietotāja statusu ar savu darba dienu administratoru.</span><span class="sxs-lookup"><span data-stu-id="10287-114">Please check the status of the Integration System user with your Workday administrator.</span></span>

<span data-ttu-id="10287-115">Lai iegūtu papildinformāciju par to, kā konfigurēt darba dienu automatizētai konfigurēšanai, skatiet rakstu [apmācība: darbdienas konfigurēšana automātiskai lietotāju nodrošināšanai](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="10287-115">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
