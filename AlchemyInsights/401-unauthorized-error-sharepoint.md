---
title: 401 Uautorisert feil i SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10935"
- "9001435"
ms.openlocfilehash: ac2fe27a8e7b277bfaf18303bf5b792410a1ea6a
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539941"
---
# <a name="401-unauthorized-error-in-sharepoint"></a><span data-ttu-id="d5b61-102">401 Uautorisert feil i SharePoint</span><span class="sxs-lookup"><span data-stu-id="d5b61-102">401 Unauthorized error in SharePoint</span></span>

<span data-ttu-id="d5b61-103">Hvis du får feilmeldingen «(401) Uautorisert» i SharePoint kan den være relatert til avviklingen av TLS 1.0/1.1.</span><span class="sxs-lookup"><span data-stu-id="d5b61-103">If you receive the error "(401) Unauthorized" in SharePoint it might be related to the deprecation of TLS 1.0/1.1.</span></span> <span data-ttu-id="d5b61-104">Hvis du vil ha mer informasjon, kan du ta en titt på:</span><span class="sxs-lookup"><span data-stu-id="d5b61-104">For more info, see:</span></span>

- [<span data-ttu-id="d5b61-105">Klargjøre for TLS 1.2 i Office 365 og Office 365 GCC</span><span class="sxs-lookup"><span data-stu-id="d5b61-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [<span data-ttu-id="d5b61-106">Godkjenningsfeil oppstår hvis klienten ikke har støtte for TLS 1.2</span><span class="sxs-lookup"><span data-stu-id="d5b61-106">Authentication errors occur if client doesn't have TLS 1.2 support</span></span>](/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [<span data-ttu-id="d5b61-107">Oppdater for å aktivere TLS 1.1 og TLS 1.2 som standard sikre protokoller i WinHTTP i Windows</span><span class="sxs-lookup"><span data-stu-id="d5b61-107">Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows</span></span>](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

<span data-ttu-id="d5b61-108">Hvis brukerne er på Windows 7, må du kontrollere at de kontrollerer [TLS Cipher Suites i Windows 7](/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span><span class="sxs-lookup"><span data-stu-id="d5b61-108">If users are on Windows 7, make sure they check [TLS Cipher Suites in Windows 7](/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span></span>