---
title: Videresende e-postmeldinger via Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 3b07dd4ccc8570e77a9ce30df48f9ac987a1db71
ms.sourcegitcommit: 93292c46464ac94971d11adfb808d066ab8bc406
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/24/2021
ms.locfileid: "53117992"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="6ce65-102">Konfigurere en enhet eller et program med flere funksjoner til å sende e-post</span><span class="sxs-lookup"><span data-stu-id="6ce65-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="6ce65-103">Hvis du vil vite mer om alternativene og trinnene, kan du se [Slik konfigurerer du en enhet eller et program med flere funksjoner til å sende e-post ved hjelp av Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="6ce65-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="6ce65-104">Hvis du har en enhet eller et program som nylig sluttet å fungere, er de vanligste problemene:</span><span class="sxs-lookup"><span data-stu-id="6ce65-104">If you have a device or application that recently stopped working, the most common issues are:</span></span>

- <span data-ttu-id="6ce65-105">**Godkjenningsrelaterte feil under bruk av SMTP Auth-klientinnsending** Vi har nylig gjort noen endringer relatert til hvordan SMTP-godkjenning fungerer.</span><span class="sxs-lookup"><span data-stu-id="6ce65-105">**Authentication related errors while using SMTP Auth client submission** We recently made some changes related to how SMTP Authentication works.</span></span> <span data-ttu-id="6ce65-106">Hvis du vil ha mer informasjon om hvordan du løser problemer, kan du se delen Om godkjenning mislyktes i Løse problemer med [skrivere, skannere](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)og LOB-programmer som sender e-post ved hjelp av Microsoft 365 eller Office 365 .</span><span class="sxs-lookup"><span data-stu-id="6ce65-106">For more information about how to resolve issues, see the authentication unsuccessful section of [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).</span></span>
- <span data-ttu-id="6ce65-107">**Vi godtar bare TLS 1.2-versjonen mens du gjør en sikker tilkobling til Office 365** Hvis du bruker Sikker tilkobling (TLS), må du kontrollere at programenheten støtter TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="6ce65-107">**We accept only the TLS 1.2 version while making a secure connection to Office 365** If you're using Secure connection (TLS), make sure your application device supports TLS 1.2.</span></span> <span data-ttu-id="6ce65-108">Hvis du vil ha mer informasjon, kan du se [Klargjøre for TLS 1.2 i Office 365 og Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="6ce65-108">For more information, see [Preparing for TLS 1.2 in Office 365 and Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span></span>
 
<span data-ttu-id="6ce65-109">Hvis du vil ha andre problemer og løsninger, kan du se Løse problemer med skrivere, skannere og [LOB-programmer](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)som sender e-post ved hjelp av Microsoft 365 eller Office 365 .</span><span class="sxs-lookup"><span data-stu-id="6ce65-109">For other issues and solutions, see [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).</span></span>

<span data-ttu-id="6ce65-110">Hvis du vil se de berørte enhetene, kan du gå til [rapporten SMTP AUTH-klienter](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="6ce65-110">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span>

<span data-ttu-id="6ce65-111">**Obs!** Exchange Online ikke tar hensyn til scenarioer for masseutsendelse.</span><span class="sxs-lookup"><span data-stu-id="6ce65-111">**Note**: Exchange Online doesn't accommodate bulk-mailing scenarios.</span></span> <span data-ttu-id="6ce65-112">Hvis du vil sende masseutsendelse av kommersiell e-post (for eksempel kundenyhetsbrev), bør du bruke tredjepartsleverandører som er spesialister på disse tjenestene.</span><span class="sxs-lookup"><span data-stu-id="6ce65-112">To send bulk commercial email (for example, customer newsletters), you should use third-party providers that specialize in these services.</span></span>
