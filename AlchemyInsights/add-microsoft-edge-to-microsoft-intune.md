---
title: Legg til Microsoft Edge i Microsoft Intune
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8240"
- "9004604"
ms.openlocfilehash: d56c65910d1c2170d3e0ce9676e913663701db96
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194514"
---
# <a name="add-microsoft-edge-to-microsoft-intune"></a><span data-ttu-id="3c3ef-102">Legg til Microsoft Edge i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="3c3ef-102">Add Microsoft Edge to Microsoft Intune</span></span>

<span data-ttu-id="3c3ef-103">Hvis du skal kunne distribuere, konfigurere, overvåke og beskytte Microsoft Edge for Windows 10, må du først legge den til i Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="3c3ef-103">To be able to deploy, configure, monitor, and protect Microsoft Edge for Windows 10, you must first add it to Microsoft Intune.</span></span>

> [!IMPORTANT]
- <span data-ttu-id="3c3ef-104">Intune støtter Microsoft Edge 77 og nyere versjoner.</span><span class="sxs-lookup"><span data-stu-id="3c3ef-104">Intune supports Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="3c3ef-105">Intune oppdager eventuelle eksisterende installasjoner av Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="3c3ef-105">Intune will detect any pre-existing installations of Microsoft Edge.</span></span>
- <span data-ttu-id="3c3ef-106">Hvis Microsoft Edge er installert i brukerkontekst, overskrives installasjonen i brukerkontekst ved en systeminstallasjon.</span><span class="sxs-lookup"><span data-stu-id="3c3ef-106">If Microsoft Edge is installed in user context, a system installation will overwrite the installation in user context.</span></span>
- <span data-ttu-id="3c3ef-107">Hvis Microsoft Edge er installert i systemkontekst, rapporteres installasjonssuksesset.</span><span class="sxs-lookup"><span data-stu-id="3c3ef-107">If Microsoft Edge is installed in system context, the installation success will be reported.</span></span>
- <span data-ttu-id="3c3ef-108">Forhåndsinstallert Microsoft Edge 77 og nyere versjoner for alle kanaler i brukerkontekst, blir overskrevet med Microsoft Edge installert i systemkontekst.</span><span class="sxs-lookup"><span data-stu-id="3c3ef-108">Pre-installed Microsoft Edge 77 and later versions, for all channels in user context, will be overwritten with Microsoft Edge installed in system context.</span></span>

<span data-ttu-id="3c3ef-109">**Forutsetning**</span><span class="sxs-lookup"><span data-stu-id="3c3ef-109">**Prerequisite**</span></span>

<span data-ttu-id="3c3ef-110">Windows 10 versjon 1709 eller nyere versjoner</span><span class="sxs-lookup"><span data-stu-id="3c3ef-110">Windows 10 version 1709 or later versions</span></span>

<span data-ttu-id="3c3ef-111">**Slik legger du til Edge i Intune**</span><span class="sxs-lookup"><span data-stu-id="3c3ef-111">**Steps to add Edge to Intune**</span></span>

1. <span data-ttu-id="3c3ef-112">[Konfigurer appen i Intune.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="3c3ef-112">[Configure the app in Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
2. <span data-ttu-id="3c3ef-113">[Konfigurere appinformasjonen.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="3c3ef-113">[Configure the app information](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
3. <span data-ttu-id="3c3ef-114">[Konfigurer appinnstillingene.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="3c3ef-114">[Configure the app settings](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
4. <span data-ttu-id="3c3ef-115">[Velg omfangskodene (valgfritt).](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="3c3ef-115">[Select the scope tags (optional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
5. <span data-ttu-id="3c3ef-116">[Legg til appen.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="3c3ef-116">[Add the app](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>

<span data-ttu-id="3c3ef-117">Hvis du vil ha mer hjelp, kan du se [Feilsøking.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="3c3ef-117">For more help, see [Troubleshooting](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>




