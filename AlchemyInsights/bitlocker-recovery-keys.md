---
title: Bitlocker atkopšanas atslēgas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 8708ed76f6abe81582823c8af89db8fffef9a3c5
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505075"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="bd462-102">Piekļuve Bitlocker atkopšanas atslēgām</span><span class="sxs-lookup"><span data-stu-id="bd462-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="bd462-103">Konfigurējot Bitlocker iestatījumus Intune galapunktu aizsardzības politiku, ir iespējams definēt, vai Bitlocker atkopšanas informācija jāglabā Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="bd462-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="bd462-104">Ja šis iestatījums ir konfigurēts, saglabātajiem atkopšanas datiem jābūt redzamiem Intune administratoram kā daļa no ierīces ierakstu datiem Intune ierīču asmenī divos veidos:</span><span class="sxs-lookup"><span data-stu-id="bd462-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="bd462-105">Ierīces - Azure AD ierīces -> "Ierīce" OR ierīces -> Visas ierīces -> "Ierīce" -> atkopšanas atslēgas</span><span class="sxs-lookup"><span data-stu-id="bd462-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="bd462-106">Alternatīvi, ja pašai ierīcei ir administratīva piekļuve, atkopšanas atslēgu (paroli) var skatīt, priviliģētā komandu uzvednē izpildot šādu komandu:</span><span class="sxs-lookup"><span data-stu-id="bd462-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
<span data-ttu-id="bd462-107">Ja ierīce tika šifrēta, pirms iereģistrējat Intune, atkopšanas atslēga, iespējams, ir saistīta ar "Microsoft kontu" (MSA), kas izmantota, lai OOBE procesa laikā pierakstītos ierīcē.</span><span class="sxs-lookup"><span data-stu-id="bd462-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="bd462-108">Šādā gadījumā, piekļūstot šai MSA un pierakstoties tajā, ir jābūt parādītām ierīcēm,  https://onedrive.live.com/recoverykey kurām tika glabātas atkopšanas atslēgas.</span><span class="sxs-lookup"><span data-stu-id="bd462-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="bd462-109">Ja ierīce tika šifrēta, veicot konfigurēšanu, izmantojot domēna grupas politiku, atkopšanas informācija var tikt glabāta lokālajā Active Directory.</span><span class="sxs-lookup"><span data-stu-id="bd462-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>

<span data-ttu-id="bd462-110">Ja esat konfigurējis galapunktu aizsardzības politiku atkopšanas atslēgas glabāšanai pakalpojumā Azure Active Directory, bet konkrētas ierīces atslēga nav augšupielādēta, varat aktivizēt augšupielādi, pagriežot šīs ierīces atkopšanas atslēgu no MEM konsoles.</span><span class="sxs-lookup"><span data-stu-id="bd462-110">If you have configured Endpoint protection policy to store the recovery key in Azure Active Directory but the key for a specific device has not been uploaded, you can trigger the upload by rotating the recovery key for that device from the MEM console.</span></span> <span data-ttu-id="bd462-111">Detalizētu informāciju skatiet rakstā [BitLocker atkopšanas atslēgu pagriešana.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)</span><span class="sxs-lookup"><span data-stu-id="bd462-111">For details, see [Rotate BitLocker recovery keys](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span></span>

