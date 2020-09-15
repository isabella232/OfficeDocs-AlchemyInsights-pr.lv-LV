---
title: BitLocker atkopšanas atslēgas
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
ms.openlocfilehash: 7c56e68cf303939d8e7d4ee0a7301e367ecfe9f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685893"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="48677-102">Piekļuve BitLocker atkopšanas taustiņiem</span><span class="sxs-lookup"><span data-stu-id="48677-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="48677-103">Konfigurējot BitLocker iestatījumu Intune galapunktu aizsardzības politiku, ir iespējams definēt, vai BitLocker atkopšanas informācija ir jāglabā Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="48677-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="48677-104">Ja šis iestatījums ir konfigurēts, saglabātajiem atkopšanas datiem ir jābūt redzamiem Intune administrators kā daļa no ierīces ieraksta datiem Intune ierīces diskam divējādi:</span><span class="sxs-lookup"><span data-stu-id="48677-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="48677-105">Ierīces — Azure AD ierīces — > "ierīce" vai ierīces-> visas ierīces-> "ierīce" — > atkopšanas atslēgas</span><span class="sxs-lookup"><span data-stu-id="48677-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="48677-106">Vai arī, ja pastāv administratora piekļuve pašai ierīcei, atkopšanas atslēgu (paroli) var redzēt, izpildot šādu komandu no privileģētas komandu uzvednes:</span><span class="sxs-lookup"><span data-stu-id="48677-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="48677-107">Ja ierīce tika šifrēta pirms reģistrācijas Intune, atkopšanas atslēga var būt saistīta ar Microsoft kontu (PPL), kas tiek izmantots, lai pierakstītos ierīcē OOBE procesa laikā.</span><span class="sxs-lookup"><span data-stu-id="48677-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="48677-108">Ja tas tā bija, piekļūstot  https://onedrive.live.com/recoverykey un pierakstoties ar šo ppl, ir jāparāda ierīces, kurām ir saglabātas atkopšanas atslēgas.</span><span class="sxs-lookup"><span data-stu-id="48677-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="48677-109">Ja ierīce ir šifrēta kā konfigurācija, kas balstīta uz domēnu grupas politiku, atkopšanas informācija var būt saglabāta lokālajā Active Directory.</span><span class="sxs-lookup"><span data-stu-id="48677-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

