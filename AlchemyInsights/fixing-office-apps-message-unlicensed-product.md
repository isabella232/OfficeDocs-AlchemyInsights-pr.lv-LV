---
title: Nevar aktivizēt Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 9a33b7880aff6016ef6df88960d6f59ac9dd50382c7e99d72ca36bc3c9f344ea
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53928376"
---
# <a name="unable-to-activate-office"></a>Nevar aktivizēt Office

**Piezīme.** Ja izmantojat vecāku Windows versiju (piemēram, Windows 7), pārliecinieties, vai TLS 1.2 ir iespējots kā noklusējums. Papildinformāciju skatiet rakstā Atjaunināšana, lai [iespējotu TLS 1.1 un TLS 1.2 kā noklusējuma drošos protokolus programmā WinHTTP Windows.](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

- Pārbaudiet, vai nav beidzies jūsu abonements.
- Pārliecinieties, vai jums ir abonements, kas atļauj klienta licences, piemēram, Office 365 Business vai Business Premium, un [nodrošiniet, ka lietotājam ir piešķirta licence](/microsoft-365/admin/manage/assign-licenses-to-users).
- Pārliecinieties, ka lietotājs pierakstās Office ar kontu, kuram piešķirta licence.
- Pārbaudiet lapu [Office 365 pakalpojumu darbspēja](/office365/enterprise/view-service-health), lai uzzinātu, vai pastāv zināmas problēmas ar pakalpojumu.
- Pārbaudiet savu ugunsmūri, pretvīrusu programmatūru un starpniekservera iestatījumus, lai pārliecinātos, ka tie nebloķē Microsoft 365 lietojumprogrammu piekļuvi internetam. Lūdzu, skatiet [Office 365 vietrāžu URL un IP adrešu diapazoni](/office365/enterprise/urls-and-ip-address-ranges "Office 365 vietrāžu URL un IP adreses diapazoni").

**Padoms** Windows datoros mēs varam diagnosticēt un automātiski risināt vairākas bieži sastopamas Office pierakstīšanās problēmas. Lejupielādējiet un palaidiet  **[Microsoft atbalsta un atkopšanas palīgu](https://aka.ms/SaRA-OfficeSignInScenario)**, lai izmantotu mūsu automatizēto rīku.

Veiciet tālāk aprakstītās darbības problēmu novēršanai.

- Atveriet Office lietojumprogrammu un [izrakstieties](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) no visiem lietotāju kontiem. [Noņemiet](/microsoft-365/admin/manage/remove-licenses-from-users) un [atkārtoti piešķiriet](/microsoft-365/admin/manage/assign-licenses-to-users) Office licenci, un pēc tam [pierakstieties Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) ar attiecīgā lietotāja kontu.
- Palaidiet [aktivācijas problēmu risinātāju](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Atiestatiet Office aktivācijas stāvokli](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Atiestatiet Office aktivācijas stāvokli")
- [Veiciet Office tiešsaistes labošanu](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

Papildu problēmu novēršanas risinājumus skatiet šeit:  

- [Nelicencēts produkts un aktivizācijas kļūdas sistēmā Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [Office aktivācijas laikā tiek parādīts kļūdas ziņojums: “Atvainojamies, bet mēs nevaram pieslēgties jūsu kontam. Lūdzu, mēģiniet vēlāk."kļūda, aktivizējot Office”](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)