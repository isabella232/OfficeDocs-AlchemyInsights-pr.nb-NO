---
title: Angi ClientAccessServerEnabled til True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749982"
---
# <a name="set-clientaccessserverenabled-to-true"></a><span data-ttu-id="37800-102">Angi ClientAccessServerEnabled til True</span><span class="sxs-lookup"><span data-stu-id="37800-102">Set ClientAccessServerEnabled to True</span></span>

<span data-ttu-id="37800-103">Hvis du ikke kan åpne en kryptert e-postmelding og i stedet ser et **rpmsg-vedlegg,** utfører du følgende trinn:</span><span class="sxs-lookup"><span data-stu-id="37800-103">If you can't open an encrypted email message and instead see an **rpmsg** attachment, perform the following steps:</span></span>

1. <span data-ttu-id="37800-104">Koble til Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="37800-104">Connect to Exchange Online PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="37800-105">Hvis du vil koble til Exchange Online PowerShell, må du logge på med en global administrator- eller Exchange-administratorkonto.</span><span class="sxs-lookup"><span data-stu-id="37800-105">To connect to Exchange Online PowerShell, you must sign in using a global admin or Exchange admin account.</span></span>

   <span data-ttu-id="37800-106">a.</span><span class="sxs-lookup"><span data-stu-id="37800-106">a.</span></span> <span data-ttu-id="37800-107">Åpne Windows PowerShell, og kjør deretter følgende kommando: `$UserCredential = Get-Credential`</span><span class="sxs-lookup"><span data-stu-id="37800-107">Open Windows PowerShell, and then run the following command: `$UserCredential = Get-Credential`</span></span>
<span data-ttu-id="37800-108">b.</span><span class="sxs-lookup"><span data-stu-id="37800-108">b.</span></span> <span data-ttu-id="37800-109">Skriv inn jobb- eller skolekontoen og passordet ditt i dialogboksen Legitimasjonsforespørsel for **Windows PowerShell,** c.</span><span class="sxs-lookup"><span data-stu-id="37800-109">In the **Windows PowerShell Credential Request** dialog box, enter your work or school account and password, c.</span></span> <span data-ttu-id="37800-110">Klikk **OK**.</span><span class="sxs-lookup"><span data-stu-id="37800-110">Click **OK**.</span></span> 

2. <span data-ttu-id="37800-111">Kjør følgende kommando for å opprette en ny økt:</span><span class="sxs-lookup"><span data-stu-id="37800-111">Run the following command to create a new session:</span></span>

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="37800-112">a.</span><span class="sxs-lookup"><span data-stu-id="37800-112">a.</span></span> <span data-ttu-id="37800-113">Kjør følgende kommando:</span><span class="sxs-lookup"><span data-stu-id="37800-113">Run the following command:</span></span>
    
    `Import-PSSession $Session -DisableNameChecking`

3. <span data-ttu-id="37800-114">Kjør `Get-IRMConfiguration` kommando.</span><span class="sxs-lookup"><span data-stu-id="37800-114">Run `Get-IRMConfiguration` command.</span></span>

4. <span data-ttu-id="37800-115">Kontroller **ClientAccessServerEnabled-innstillingen.**</span><span class="sxs-lookup"><span data-stu-id="37800-115">Check the **ClientAccessServerEnabled** setting.</span></span> 

    <span data-ttu-id="37800-116">a.</span><span class="sxs-lookup"><span data-stu-id="37800-116">a.</span></span> <span data-ttu-id="37800-117">Hvis **ClientAccessServerEnabled-innstillingen** er satt til **False**, kjører du følgende cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span><span class="sxs-lookup"><span data-stu-id="37800-117">If **ClientAccessServerEnabled** setting is set to **False**, run the following cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span></span>

> [!TIP]
> <span data-ttu-id="37800-118">Lukk alltid PowerShell-økten med følgende kommando: `Remove-PSSession $Session`</span><span class="sxs-lookup"><span data-stu-id="37800-118">Always close your powershell session with the following command: `Remove-PSSession $Session`</span></span>

<span data-ttu-id="37800-119">Hvis du vil ha mer informasjon, kan du [se Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="37800-119">For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

