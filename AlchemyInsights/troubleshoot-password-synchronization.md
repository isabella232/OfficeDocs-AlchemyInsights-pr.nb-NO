---
title: Feilsøke passord synkronisering
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664935"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="f84e4-102">Feilsøke passord synkronisering</span><span class="sxs-lookup"><span data-stu-id="f84e4-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="f84e4-103">Hvis du vil feilsøke problemer med passord synkronisering, starter du med denne oppgaven for feil søking av AAD Connect for å fastslå hvorfor passord ikke synkroniseres.</span><span class="sxs-lookup"><span data-stu-id="f84e4-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="f84e4-104">Hvis du vil begynne, kan du gå til [administrere direkte synkronisering](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="f84e4-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="f84e4-105">Åpne en ny Windows PowerShell-økt på Azure AD Connect-serveren, og velg alternativet **Kjør som administrator** .</span><span class="sxs-lookup"><span data-stu-id="f84e4-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="f84e4-106">Kjør set-ExecutionPolicy RemoteSigned eller set-ExecutionPolicy unrestricted.</span><span class="sxs-lookup"><span data-stu-id="f84e4-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="f84e4-107">Start vei viseren for Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="f84e4-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="f84e4-108">Gå til siden for flere aktiviteter > **Feilsøke**  >  **neste**.</span><span class="sxs-lookup"><span data-stu-id="f84e4-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="f84e4-109">Velg **Start** for å åpne menyen for feil søking av PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f84e4-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="f84e4-110">Velg **Feilsøk passord synkronisering**.</span><span class="sxs-lookup"><span data-stu-id="f84e4-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="f84e4-111">Problemet er vanligvis at et passord ikke er synkronisert for en bestemt bruker konto.</span><span class="sxs-lookup"><span data-stu-id="f84e4-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="f84e4-112">**Notater** Passord synkronisering mislykkes hvis den siste vellykkede synkroniseringen av passord var en tid siden.</span><span class="sxs-lookup"><span data-stu-id="f84e4-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="f84e4-113">Hvis du vil ha mer informasjon om feil søking av passord, kan du se [Feilsøke passord nummer synkronisering med Azure ad Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)-synkronisering.</span><span class="sxs-lookup"><span data-stu-id="f84e4-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>