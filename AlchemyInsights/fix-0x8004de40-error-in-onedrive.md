---
title: Løse 0x8004de40 i OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649757"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="1a8bb-102">Løse 0x8004de40 i OneDrive</span><span class="sxs-lookup"><span data-stu-id="1a8bb-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="1a8bb-103">Hvis du kjører Windows 7 og får denne feilen, oppdaterer [du TLS 1.1 og TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)som standard sikre protokoller i WinHTTP i Windows .</span><span class="sxs-lookup"><span data-stu-id="1a8bb-103">If you're running Windows 7 and receive this error, [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

<span data-ttu-id="1a8bb-104">Hvis du kjører Windows 10, og du får en 0x8004de40 feilmelding med OneDrive:</span><span class="sxs-lookup"><span data-stu-id="1a8bb-104">If you're running Windows 10, and you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="1a8bb-105">Start den berørte datamaskinen på nytt mens du er koblet til Acitve Directory-domenet.</span><span class="sxs-lookup"><span data-stu-id="1a8bb-105">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="1a8bb-106">Hvis en omstart ikke løser problemet, kan du koble til og bli med på enheten på nytt fra Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1a8bb-106">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="1a8bb-107">**Obs!** Du bør være på bedriftsnettverket mens du utfører disse trinnene.</span><span class="sxs-lookup"><span data-stu-id="1a8bb-107">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="1a8bb-108">Ikke utfør disse trinnene når du ikke er koblet til bedriftens infrastruktur (for eksempel når du er på reise).</span><span class="sxs-lookup"><span data-stu-id="1a8bb-108">Don't perform these steps when you aren't connected to your corporate infrastructure (for example, while traveling).</span></span> 

1. <span data-ttu-id="1a8bb-109">Åpne en forhøyet ledetekst ved å velge **Start**, høyreklikk **ledetekst**, og velg deretter Kjør som **administrator**.</span><span class="sxs-lookup"><span data-stu-id="1a8bb-109">Open an elevated command prompt by selecting **Start**, right-click **Command Prompt**, and then select **Run as administrator**.</span></span>

1. <span data-ttu-id="1a8bb-110">Skriv *inn dsregcmd /leave, og* trykk **ENTER**.</span><span class="sxs-lookup"><span data-stu-id="1a8bb-110">Type *dsregcmd /leave* and press **Enter**.</span></span>

1. <span data-ttu-id="1a8bb-111">Når du er ferdig, skriver du *inn dsregcmd /join og* trykker **ENTER.**</span><span class="sxs-lookup"><span data-stu-id="1a8bb-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>

1. <span data-ttu-id="1a8bb-112">Lukk ledeteksten når du er ferdig.</span><span class="sxs-lookup"><span data-stu-id="1a8bb-112">When complete, close the command prompt.</span></span>

1. <span data-ttu-id="1a8bb-113">Start datamaskinen på nytt, og logg på OneDrive.</span><span class="sxs-lookup"><span data-stu-id="1a8bb-113">Reboot the computer, and log into OneDrive.</span></span>