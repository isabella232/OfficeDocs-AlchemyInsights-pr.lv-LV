---
title: Problēmu novēršana saistībā ar sertifikātu SAML
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693425"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a><span data-ttu-id="5ab63-102">Problēmu novēršana saistībā ar sertifikātu SAML</span><span class="sxs-lookup"><span data-stu-id="5ab63-102">Troubleshoot SAML Signing certificate issues</span></span>

<span data-ttu-id="5ab63-103">Lai atrisinātu SAML pierakstīšanās sertifikāta problēmu, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="5ab63-103">To resolve SAML Signing certificate issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="5ab63-104">Kad pievienojat uzņēmuma lietojumprogrammu, kas atbalsta SSO, Azure ģenerēs sertifikātu, ko dēvē par [SAML parakstīšanas sertifikātu](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span><span class="sxs-lookup"><span data-stu-id="5ab63-104">When you add an enterprise application which supports SSO, Azure will generate a certificate which is called the [SAML Signing certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span></span> <span data-ttu-id="5ab63-105">Šī sertifikāta derīguma termiņš ir 3 gadi.</span><span class="sxs-lookup"><span data-stu-id="5ab63-105">This certificate has an expiration date of 3 years.</span></span> <span data-ttu-id="5ab63-106">Lai mainītu sertifikāta derīguma termiņu, skatiet rakstu [Federācijas sertifikāta derīguma termiņa pielāgošana un pāriešana uz jaunu sertifikātu](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span><span class="sxs-lookup"><span data-stu-id="5ab63-106">To change the expiration date of your certificate, see [Customize the expiration date for your federation certificate and roll it over to a new certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span></span>
2. <span data-ttu-id="5ab63-107">Azure izmantos šo sertifikātu, lai parakstītu SAML marķierus, kurus pieprasījusi lietojumprogramma, un nosūtītu to uz lietojumprogrammas izraudzīto SSO.</span><span class="sxs-lookup"><span data-stu-id="5ab63-107">Azure will use this certificate to sign the SAML tokens requested by the application and send it over to the application for a successful SSO.</span></span> <span data-ttu-id="5ab63-108">Lai šo pabeigtu, lejupielādējiet sertifikātu no Azure portāla un nosūtiet to lietojumprogrammas piedāvātājam, lai pabeigtu SSO procesu.</span><span class="sxs-lookup"><span data-stu-id="5ab63-108">In order for this to complete, download the certificate from the Azure portal and send it to the application vendor to complete the SSO process.</span></span>

<span data-ttu-id="5ab63-109">Pēc tam, kad šī procesa pabeigšana lietojumprogramma uzticēs šo sertifikātu un visas šajā sertifikātā parakstītās SAML marķierierīces tiks akceptētas.</span><span class="sxs-lookup"><span data-stu-id="5ab63-109">After this process completes your application will trust this certificate and all the SAML tokens signed by this certificate will be accepted by the application.</span></span>

3. <span data-ttu-id="5ab63-110">Ja šī sertifikāta derīgums beidzas, izveidojiet jaunu sertifikātu, atjauniniet to lietojumprogrammas pārdevējam un pēc tam aktivizējiet to pakalpojumā Azure Side.</span><span class="sxs-lookup"><span data-stu-id="5ab63-110">If this certificate expires, create a new certificate, update it to the application vendor and then make it active on the Azure side.</span></span> <span data-ttu-id="5ab63-111">Papildinformāciju skatiet rakstā [tā sertifikāta atjaunošana, kura derīguma termiņš drīz beigsies](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span><span class="sxs-lookup"><span data-stu-id="5ab63-111">For more information, see [Renew a certificate that will soon expire](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span></span>

> [!NOTE]
> <span data-ttu-id="5ab63-112">Ja sertifikāta derīgums beidzas, lietotājs netiks bloķēts.</span><span class="sxs-lookup"><span data-stu-id="5ab63-112">If the certificate expires, the user will not be blocked.</span></span>

4. <span data-ttu-id="5ab63-113">[Pievienojiet e-pasta adresi paziņojumiem](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) , kas tiks saņemti pirms pašreizējā sertifikāta derīguma perioda beigām.</span><span class="sxs-lookup"><span data-stu-id="5ab63-113">[Add an email address for notifications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) to be received before the current certificate expires.</span></span>

> [!NOTE]
> <span data-ttu-id="5ab63-114">Step-4 nav obligāts.</span><span class="sxs-lookup"><span data-stu-id="5ab63-114">Step-4 is an optional one.</span></span>

5. <span data-ttu-id="5ab63-115">Mainiet lietojumprogrammas SAML sertifikāta parakstīšanas opcijas un sertifikāta parakstīšanas algoritmu.</span><span class="sxs-lookup"><span data-stu-id="5ab63-115">Change an application's SAML certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="5ab63-116">Papildinformāciju skatiet rakstā [sertifikāta parakstīšanas opciju un paraksta algoritma maiņa](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span><span class="sxs-lookup"><span data-stu-id="5ab63-116">For more information, see [Change certificate signing options and signing algorithm](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>

