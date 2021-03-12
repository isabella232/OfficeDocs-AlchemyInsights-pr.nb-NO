---
title: Aktivere Microsoft Defender for Office 365 for SharePoint Online, OneDrive og Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747746"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="2b715-102">Aktivere Microsoft Defender for Office 365 for SharePoint Online, OneDrive og Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="2b715-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive and Microsoft Teams</span></span>

1. <span data-ttu-id="2b715-103">Bruk den globale administrator- eller sikkerhetsadministratorlegitimasjonen til å logge på sikkerhets- og samsvarssenteret for [Office 365.](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="2b715-103">Using your global admin or security admin credentials, log in to the [Office 365 Security and Compliance Center](https://protection.office.com/).</span></span>
2. <span data-ttu-id="2b715-104">Velg **Trusselbehandling** i den venstre ruten, og velg deretter **Policysikkert**  >  [vedlegg](https://protection.office.com/safeattachment).</span><span class="sxs-lookup"><span data-stu-id="2b715-104">Select **Threat management** in the left pane, and then select **Policy** > [Safe attachments](https://protection.office.com/safeattachment).</span></span>
3. <span data-ttu-id="2b715-105">Velg **Slå på Microsoft Defender for Office 365 for SharePoint, OneDrive** og Microsoft Teams, og velg deretter **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="2b715-105">Select **Turn on Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then select **Save**.</span></span>
    > [!TIP]
    >
    > - <span data-ttu-id="2b715-106">Som global administrator eller SharePoint Online-administrator kjører du følgende PowerShell-cmdlet med **parameteren DisallowInfectedFileDownload** satt til *sann:* [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span><span class="sxs-lookup"><span data-stu-id="2b715-106">As a global admin or a SharePoint Online admin, run the following PowerShell cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span></span>
    > - [<span data-ttu-id="2b715-107">Konfigurere varsler for oppdagede filer</span><span class="sxs-lookup"><span data-stu-id="2b715-107">Set up alerts for detected files</span></span>](https://go.microsoft.com/fwlink/?linkid=2092110)

<span data-ttu-id="2b715-108">Hvis du vil ha mer informasjon, kan du se [Microsoft Defender for Office 365 for SharePoint, OneDrive og Microsoft Teams.](https://go.microsoft.com/fwlink/?linkid=2092041)</span><span class="sxs-lookup"><span data-stu-id="2b715-108">For more information, see [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).</span></span>
