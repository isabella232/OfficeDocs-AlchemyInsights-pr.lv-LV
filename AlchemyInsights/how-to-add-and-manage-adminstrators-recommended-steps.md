---
title: Administratoru pievienošana un pārvaldība — ieteicamās darbības
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: 48a06fde215e007b6b81b32ab751ca8e4bba522d
ms.sourcegitcommit: 46e24d65cffd37b6988447c6738b3315303bbe13
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/13/2021
ms.locfileid: "58339039"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>Administratoru pievienošana un pārvaldība — ieteicamās darbības

Ņemot vērā jūsu problēmas aprakstu, esam atraduši jums risinājumu. Lielākajai daļai klientu problēma tika novērsta paši pēc mūsu dokumentācijas sekošanas.

**Rediģēt abonementa administratoru vai līdz administratoru**

- Konta administrators var rediģēt abas lomas, bet abonementa administrators Var mainīt tikai līdzadministratoriem [Azure portālā.](https://ms.portal.azure.com/#home)
- [Azure abonementa administratoru pievienošana vai maiņa](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Atjaunināt abonementa administratoru vai Co-Administrator iekšējām (AIRS) abonementiem**

Pakalpojumu administrators vai līdz administrators var paši veikt šo darbību, veicot tālāk norādītās darbības.

1. Piesakieties [Azure portālā un kreisajā](https://ms.portal.azure.com/#home) **asī noklikšķiniet** uz Izmaksu pārvaldība + Norēķini.
2. Noklikšķiniet uz rindas vienuma ar jūsu abonementu. Tiek atvērts jūsu abonementa pārskats.
3. Abonementa **asmens** izvēlnē noklikšķiniet uz **Rekvizīti**. 
4. Noklikšķiniet uz **pogas Pakalpojumu** administrators.
5. Ievadiet tā lietotāja e-pasta adresi, kuru vēlaties iestatīt kā pakalpojuma administratoru, un noklikšķiniet uz **Labi.**

**Līdz administratoru pievienošana/mainīšana/noņemšana**

1. Piesakieties [Azure portālā](https://ms.portal.azure.com/#home) kā pakalpojumu administrators.
2. Atveriet [abonementus](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) un atlasiet abonementu. (Līdz administratorus var piešķirt tikai abonementa tvērumā.)
3. Naviģējiet uz Access vadības **(IAM)** klasiskie administratori Pievienot līdzadministratoriem, lai atvērtu līdzadministratoriem pievienošanas rūti (ja opcija Pievienot līdzadministratoriem ir atspējota, tas norāda, ka jums nav  >    >    >   atļauju). 
4. Atlasiet lietotāju, kuru vēlaties pievienot, un noklikšķiniet uz **Pievienot.**

**Papildinformācija:**
- [Līdz administratoru pievienošana](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Administratora noņemšana](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Pakalpojumu administratora maiņa](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Skatīt konta administratoru](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Piekļuves pārvaldība, izmantojot RBAC un Azure portālu](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Lietotāju pievienošana/dzēšana, izmantojot Azure Active Directory (AD)**

Varat pievienot jaunus lietotājus vai izdzēst esošos lietotājus no savas Azure Active Directory (Azure AD) organizācijas:

1. Lai pievienotu jaunu lietotāju, [piesakieties Azure portālā](https://ms.portal.azure.com/#home) kā organizācijas lietotāja administrators.
2. Atlasiet **Azure Active Directory**, atlasiet **Lietotāji un** pēc tam noklikšķiniet uz Jauns **lietotājs.**
3. Aizpildiet  nepieciešamo informāciju lapā Lietotājs. Noklikšķiniet **uz Izveidot.** Lietotājs tiek izveidots un pievienots jūsu Azure AD nomniekam.

**Papildinformācija:**

- [Jauna lietotāja pievienošana](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Lietotāja dzēšana](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Lietotāja profila informācijas pievienošana vai atjaunināšana, izmantojot Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Ieteiktie dokumenti**

- [Kas ir lomu piekļuves vadība (role-based access control — RBAC)?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Dažādu lomu izpratne programmā Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Administratora lomu atļaujas programmā Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Apmācība: piekļuves piešķiršana lietotājam, izmantojot RBAC un Azure portālu](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [RBAC problēmu novēršana programmā Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Resursu organizēšana, izmantojot Azure pārvaldības grupas](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Kā pieprasīt Azure rēķina kopiju pa e-pastu](https://azure.microsoft.com/blog/azure-email-invoices/)
- [Kā pievienot, atjaunināt vai noņemt kredītkarti vai debetkarti no Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Abonementa pārvaldība (atkārtota aktivizēšana/atcelšana/pārslēgšana)](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



