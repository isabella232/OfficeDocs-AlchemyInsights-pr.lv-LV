---
title: Microsoft Defender for Office 365 pretpikšķerēšanas politikas piemērs
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694034"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a><span data-ttu-id="26636-102">Microsoft Defender for Office 365 pretpikšķerēšanas politikas piemērs</span><span class="sxs-lookup"><span data-stu-id="26636-102">Example Microsoft Defender for Office 365 anti-phishing policy</span></span>

<span data-ttu-id="26636-103">Šie iestatījumi iespējo politiku ar nosaukumu *Domain un CEO*.</span><span class="sxs-lookup"><span data-stu-id="26636-103">These settings enable a policy called *Domain and CEO*.</span></span> <span data-ttu-id="26636-104">Šī politika nodrošina gan lietotāja, gan domēna aizsardzību no personificēšanas un pēc tam lieto politiku visiem lietotājiem, kas ir saņemti domēnā.</span><span class="sxs-lookup"><span data-stu-id="26636-104">This policy provides both user and domain protection from impersonation and then applies the policy to all email received by users within the domain.</span></span> <span data-ttu-id="26636-105">Vispirms pievienojiet tālāk norādīto informāciju, lai izveidotu politiku.</span><span class="sxs-lookup"><span data-stu-id="26636-105">First, add the following information to create the policy:</span></span>

- <span data-ttu-id="26636-106">**Nosaukums**: Domain and CEO **Apraksts**: nodrošina, ka vadītājs un jūsu domēns netiek personificēts.</span><span class="sxs-lookup"><span data-stu-id="26636-106">**Name**: Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.</span></span>
  <span data-ttu-id="26636-107">**Lietots**: atlasiet **adresātu domēnu**.</span><span class="sxs-lookup"><span data-stu-id="26636-107">**Applied to**: Select **The recipient domain is**.</span></span> <span data-ttu-id="26636-108">Sadaļā **jebkurš no šiem** atlasiet **izvēlēties** un pēc tam atlasiet domēnu.</span><span class="sxs-lookup"><span data-stu-id="26636-108">Under **Any of these**, select **Choose**, and then select a domain.</span></span> <span data-ttu-id="26636-109">Atlasiet **+ Pievienot**.</span><span class="sxs-lookup"><span data-stu-id="26636-109">Select **+ Add**.</span></span> <span data-ttu-id="26636-110">Atzīmējiet izvēles rūtiņu blakus domēna nosaukumam sarakstā (piemēram, *contoso.com*) un pēc tam atlasiet **Pievienot**.</span><span class="sxs-lookup"><span data-stu-id="26636-110">Select the check box next to the name of the domain in the list (for example, *contoso.com*), and then select **Add**.</span></span> <span data-ttu-id="26636-111">Atlasiet **gatavs**.</span><span class="sxs-lookup"><span data-stu-id="26636-111">Select **Done**.</span></span>
- <span data-ttu-id="26636-112">Pēc politikas izveides varat precizēt politiku, izmantojot tālāk norādītās opcijas.</span><span class="sxs-lookup"><span data-stu-id="26636-112">After the policy is created, you can fine-tune the policy by using the following options:</span></span>
  - <span data-ttu-id="26636-113">**Lietotāju pievienošana aizsardzībai:** Šim piemēram, pievienojiet izpilddirektora e-pasta adresi.</span><span class="sxs-lookup"><span data-stu-id="26636-113">**Add users to protect:** For this example, add the CEO's email address, at a minimum.</span></span>
  - <span data-ttu-id="26636-114">**Pievienot domēnus, lai aizsargātu**: pievienojiet organizācijas domēnu, kas ietver CEO biroju.</span><span class="sxs-lookup"><span data-stu-id="26636-114">**Add domains to protect**: Add the organizational domain that includes the office of the CEO.</span></span>
  - <span data-ttu-id="26636-115">**Izvēlieties darbības**: **Ja e-pasta ziņojums tiek nosūtīts personificētam lietotājam**, atlasiet **novirzīt ziņojumu uz citu e-pasta adresi** un pēc tam ievadiet drošības administratora e-pasta adresi (piemēram, *SecurityAdmin@contoso.com*).</span><span class="sxs-lookup"><span data-stu-id="26636-115">**Choose actions**: For **If email is sent by an impersonated user**, select **Redirect message to another email address**, and then enter the email address of the security administrator (for example, *securityadmin@contoso.com*).</span></span> <span data-ttu-id="26636-116">**Ja e-pasta ziņojums tiek sūtīts ar personificētu domēnu**, atlasiet **ievietot ziņojumu karantīnā**.</span><span class="sxs-lookup"><span data-stu-id="26636-116">For **If email is sent by an impersonated domain**, select **Quarantine the message**.</span></span>
  - <span data-ttu-id="26636-117">**Pastkastes informācija**: pēc noklusējuma šī opcija ir atlasīta, kad izveidojat jaunu pretpikšķerēšanas politiku.</span><span class="sxs-lookup"><span data-stu-id="26636-117">**Mailbox intelligence**: By default, this option is selected when you create a new anti-phishing policy.</span></span> <span data-ttu-id="26636-118">Atstājiet **šo iestatījumu,** lai iegūtu vislabākos rezultātus.</span><span class="sxs-lookup"><span data-stu-id="26636-118">Leave this setting **On** for best results.</span></span>
  - <span data-ttu-id="26636-119">**Pievienojiet uzticamos sūtītājus un domēnus:** Šajā piemērā nedefinējiet nevienu ignorēšanu.</span><span class="sxs-lookup"><span data-stu-id="26636-119">**Add trusted senders and domains:** For this example, don't define any overrides.</span></span>
- <span data-ttu-id="26636-120">Kad būsit pārskatījis savus iestatījumus, atlasiet **izveidot šo politiku** vai pēc vajadzības **Saglabāt**.</span><span class="sxs-lookup"><span data-stu-id="26636-120">Once you've reviewed your settings, select **Create this policy** or **Save**, as appropriate.</span></span>

<span data-ttu-id="26636-121">Papildinformāciju skatiet rakstā [pretpikšķerēšanas politikas programmā Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span><span class="sxs-lookup"><span data-stu-id="26636-121">To learn more, see [Anti-phishing policies in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span></span>
