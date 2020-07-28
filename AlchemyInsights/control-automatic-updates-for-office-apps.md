---
title: Kontrollere automatiske oppdateringer for Office Apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439931"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="81753-102">Kontrollere automatiske oppdateringer for Office Apps</span><span class="sxs-lookup"><span data-stu-id="81753-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="81753-103">Som standard lastes oppdateringer for Office Apps ned automatisk og brukes i bakgrunnen uten brukermedvirkning.</span><span class="sxs-lookup"><span data-stu-id="81753-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="81753-104">Administratorer kan imidlertid kontrollere hvordan oppdateringer brukes ved hjelp av Office Update-innstillinger.</span><span class="sxs-lookup"><span data-stu-id="81753-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="81753-105">Oppdateringsinnstillinger gjør det mulig for administratorer å aktivere eller deaktivere automatiske oppdateringer, vise eller skjule **Oppdater nå-knappen** i Office, angi oppdateringsfrister og mer.</span><span class="sxs-lookup"><span data-stu-id="81753-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="81753-106">Hvis du vil ha detaljert informasjon, kan du se:</span><span class="sxs-lookup"><span data-stu-id="81753-106">For detailed information, see:</span></span>

- [<span data-ttu-id="81753-107">Konfigurere oppdateringsinnstillinger for Office</span><span class="sxs-lookup"><span data-stu-id="81753-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="81753-108">Automatisk oppdatering for Office er ikke aktivert</span><span class="sxs-lookup"><span data-stu-id="81753-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="81753-109">Definere hvordan Office oppdateres etter at det er installert</span><span class="sxs-lookup"><span data-stu-id="81753-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="81753-110">Hvis du vil se gjennom de eksisterende oppdateringsinnstillingene som brukes på en klientmaskin, gjør du følgende:</span><span class="sxs-lookup"><span data-stu-id="81753-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="81753-111">Åpne Registerredigering ved å gå til **Start**  >  **Kjør**  >  **regedit**.</span><span class="sxs-lookup"><span data-stu-id="81753-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="81753-112">Bytt til følgende plassering, og se gjennom Office Update-innstillingene:</span><span class="sxs-lookup"><span data-stu-id="81753-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="81753-113">a.</span><span class="sxs-lookup"><span data-stu-id="81753-113">a.</span></span> <span data-ttu-id="81753-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span><span class="sxs-lookup"><span data-stu-id="81753-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="81753-115">b.</span><span class="sxs-lookup"><span data-stu-id="81753-115">b.</span></span> <span data-ttu-id="81753-116">KlikkToRun\Konfigurasjon</span><span class="sxs-lookup"><span data-stu-id="81753-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="81753-117">**Merk at**  Hvis OfficeMgmtCOM-nøkkelen er angitt, kan du se meldingen "Oppdateringer **Office**administreres av systemansvarlig" i  >  **Office-konto**  >  **Office-oppdateringer**.</span><span class="sxs-lookup"><span data-stu-id="81753-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="81753-118">Hvis du vil ha mer informasjon, kan du se [Administrere oppdateringer for Microsoft 365-apper med Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="81753-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  