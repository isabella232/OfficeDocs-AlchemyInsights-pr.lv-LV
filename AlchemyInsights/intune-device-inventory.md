---
title: Intune ierīces noliktava
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439657"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="7cbe0-102">Intune ierīces noliktava</span><span class="sxs-lookup"><span data-stu-id="7cbe0-102">Intune Device Inventory</span></span>

<span data-ttu-id="7cbe0-103">Ierīču asmens sniedz administratora ieskatu par ierīcēm, kas ir iekļautas pārvaldības Intune ierīcē katrai ierīcei.</span><span class="sxs-lookup"><span data-stu-id="7cbe0-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="7cbe0-104">Parādītajā informācijā ietilpst: aparatūra, atklātās lietojumprogrammas, ierīces atbilstības stāvoklis un ierīces konfigurācijas stāvoklis.</span><span class="sxs-lookup"><span data-stu-id="7cbe0-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="7cbe0-105">Aparatūras un atklāto lietojumprogrammu inventarizācijas dati tiek apkopoti septiņu dienu ciklā.</span><span class="sxs-lookup"><span data-stu-id="7cbe0-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="7cbe0-106">Ziņotās aparatūras lietojumprogrammas un īpašie elementi atšķiras atkarībā no ierīces operētājsistēmas un tā, vai ierīce ir personiski vai uzņēmuma īpašumā.</span><span class="sxs-lookup"><span data-stu-id="7cbe0-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="7cbe0-107">Papildinformāciju skatiet rakstā [ierīces datu skatīšana Intune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="7cbe0-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="7cbe0-108">**BUJ**</span><span class="sxs-lookup"><span data-stu-id="7cbe0-108">**FAQ**</span></span>

<span data-ttu-id="7cbe0-109">Jautājums: Es nesaņemu pilnu sarakstu ar lietojumprogrammām, kas ir iekļautas Intune Windows ierīcēs.</span><span class="sxs-lookup"><span data-stu-id="7cbe0-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="7cbe0-110">kāpēc ne?</span><span class="sxs-lookup"><span data-stu-id="7cbe0-110">Why not?</span></span>

<span data-ttu-id="7cbe0-111">A: šajā laikā ir norādītas tikai modernās lietojumprogrammas, kas paredzētas Windows 10 datoriem, kas ir identificēti kā korporatīvās ierīces.</span><span class="sxs-lookup"><span data-stu-id="7cbe0-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="7cbe0-112">Intune neapkopo informāciju par šajās ierīcēs instalētajām Win32 programmām.</span><span class="sxs-lookup"><span data-stu-id="7cbe0-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="7cbe0-113">J: Kāpēc tālruņu numuri nav apkopoti no visām ierīcēm?</span><span class="sxs-lookup"><span data-stu-id="7cbe0-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="7cbe0-114">A: tālruņi, kas iedalīti kā korporatīvās ierīces pakalpojumā Intune, netiek identificēti ar pilnu tālruņa numuru, piemēram, varat izpildīt mobilo ierīču inventarizācijas atskaiti.</span><span class="sxs-lookup"><span data-stu-id="7cbe0-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="7cbe0-115">No jūsu ierīces tālruņa numuri vienmēr tiek daļēji maskēti ar zvaigznītēm (\* \* \* \* \*) un tiek parādīti tikai pēdējie četri cipari.</span><span class="sxs-lookup"><span data-stu-id="7cbe0-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>