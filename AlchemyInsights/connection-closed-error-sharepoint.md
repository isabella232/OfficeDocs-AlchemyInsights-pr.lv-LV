---
title: Pamatā esošais savienojums tika slēgts SharePoint
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: 101c0ba90d2bec6b1684fd63645ba2f8f89783ad5bfdf0efe739d31dfd951f66
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044419"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>Kļūdas ziņojums "Pamatā esošais savienojums tika aizvērts" SharePoint

Ja saņemat kļūdas ziņojumu "Pamatā esošais savienojums tika aizvērts" SharePoint tas, iespējams, ir saistīts ar TLS 1.0/1.1 novecošanu. Papildinformāciju skatiet šajos rakstos:

- [Gatavošanās TLS 1.2 Office 365 Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Autentifikācijas kļūdas rodas, ja klientam nav TLS 1.2 atbalsta](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Atjauniniet, lai iespējotu TLS 1.1 un TLS 1.2 kā noklusējuma drošo protokolu winhttp Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Ja lietotāji izmanto 7 Windows, pārliecinieties, vai viņi [pārbauda TLS cipher Suite in Windows 7.](/windows/win32/secauthn/tls-cipher-suites-in-windows-7)