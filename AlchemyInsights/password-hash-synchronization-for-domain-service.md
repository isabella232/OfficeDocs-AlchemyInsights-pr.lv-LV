---
title: Paroļu jaukšanas sinhronizācija domēna pakalpojumam
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177487"
---
# <a name="password-hash-synchronization-for-domain-service"></a>Paroļu jaukšanas sinhronizācija domēna pakalpojumam

**Ja jūsu Azure AD DS instance piedāvā iespējot paroļu jaukšanas sinhronizāciju**

Tiek parādīts scenārijs, kurā tiek palaista Hibrīdā vide ar lietotājiem, kas tiek sinhronizēti no lokālā Azure Active Directory domēna pakalpojumu (AD DS) vides. Šis scenārijs ir sastopams, ja jums ir paroļu jaukšanas sinhronizācija no lokālā AD DS uz jūsu Azure AD nomnieku.

**Izraisīt**

Tas notiek tāpēc, ka Azure AD Connect pēc noklusējuma nesinhronizē mantoto jauno tehnoloģiju LAN Manager (NTLM) un Kerberos paroļu hashes, kas nepieciešamas Azure AD DS lietošanai.

**Risinājums** 

Lai sinhronizētu šīs paroļu hashes, kas nepieciešami NTLM un Kerberos autentifikācijai, ir jākonfigurē Azure AD Connect.

Pēc Azure AD Connect konfigurēšanas, lokālā konta izveides vai paroles maiņas notikums arī pēc tam sinhronizē mantotās paroļu jaucējvirknes uz Azure AD. Lai iegūtu papildinformāciju par šo problēmu, skatiet [šeit](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) un norādījumus par to, kā iespējot paroļu SINHRONIZĀCIJU AZURE AD DS hibrīdās vidēs.