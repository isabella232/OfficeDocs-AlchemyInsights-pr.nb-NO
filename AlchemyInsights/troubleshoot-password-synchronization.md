---
title: Feilsøke synkronisering av passord
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387886"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="9a49a-102">Feilsøke synkronisering av passord</span><span class="sxs-lookup"><span data-stu-id="9a49a-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="9a49a-103">Hvis du vil feilsøke problemer med synkronisering av passord, starter du ved hjelp av denne feilsøkingsoppgaven for AAD Connect for å finne ut hvorfor passord ikke synkroniseres.</span><span class="sxs-lookup"><span data-stu-id="9a49a-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="9a49a-104">Du begynner ved å gå til [Behandle direkte synkronisering](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="9a49a-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="9a49a-105">Åpne en ny Windows PowerShell-økt på Azure AD Connect-serveren, og velg alternativet **Kjør som administrator.**</span><span class="sxs-lookup"><span data-stu-id="9a49a-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="9a49a-106">Kjør Set-ExecutionPolicy RemoteSigned eller Set-ExecutionPolicy Ubegrenset.</span><span class="sxs-lookup"><span data-stu-id="9a49a-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="9a49a-107">Start azure AD Connect-veiviseren.</span><span class="sxs-lookup"><span data-stu-id="9a49a-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="9a49a-108">Gå til siden Flere oppgaver > **Feilsøke**  >  **neste**.</span><span class="sxs-lookup"><span data-stu-id="9a49a-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="9a49a-109">Velg **Start** for å åpne feilsøkingsmenyen for PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9a49a-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="9a49a-110">Velg **Feilsøke synkronisering av passord**.</span><span class="sxs-lookup"><span data-stu-id="9a49a-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="9a49a-111">Problemet er vanligvis at et passord ikke synkroniseres for en bestemt brukerkonto.</span><span class="sxs-lookup"><span data-stu-id="9a49a-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="9a49a-112">**Notater** Synkronisering av passord mislykkes hvis den siste vellykkede synkroniseringen av passord var for en tid siden.</span><span class="sxs-lookup"><span data-stu-id="9a49a-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="9a49a-113">Hvis du vil ha mer hjelp med feilsøking av synkronisering av passord, kan du se [Feilsøke synkronisering av passordhash med Azure AD Connect-synkronisering](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="9a49a-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>