---
title: Tilbakeskriving av passord fungerer ikke
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243517"
---
# <a name="password-writeback-is-not-working"></a><span data-ttu-id="d6610-102">Tilbakeskriving av passord fungerer ikke</span><span class="sxs-lookup"><span data-stu-id="d6610-102">Password Writeback is not working</span></span>

<span data-ttu-id="d6610-103">**Jeg har problemer med å konfigurere tilbakeskriving av passord**</span><span class="sxs-lookup"><span data-stu-id="d6610-103">**I'm having problems configuring password writeback**</span></span>

- <span data-ttu-id="d6610-104">Tilbakeskriving av passord er en premiumfunksjon.</span><span class="sxs-lookup"><span data-stu-id="d6610-104">Password writeback is a premium feature.</span></span>
- <span data-ttu-id="d6610-105">Kontroller at du forstår lisensieringskravene:</span><span class="sxs-lookup"><span data-stu-id="d6610-105">Make sure that you understand the licensing requirements:</span></span>
  - <span data-ttu-id="d6610-106">Du må ha minst én lisens tilordnet i organisasjonen</span><span class="sxs-lookup"><span data-stu-id="d6610-106">You must have at least one license assigned in your organization</span></span>
  - <span data-ttu-id="d6610-107">**Bare skybrukere** – alle Office 365 (O365) betalte SKU-er, eller Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="d6610-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
  - <span data-ttu-id="d6610-108">**Skybrukere og/eller** lokale brukere – Azure AD Premium P1 eller P2, Enterprise Mobility + Security (EMS) eller Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="d6610-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="d6610-109">Hvis du vil finne ut mer om lisensieringskrav, kan du se Lisensieringskrav [for selvbetjent tilbakestilling av passord for Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="d6610-109">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span></span>
- <span data-ttu-id="d6610-110">Du har minst én administratorkonto og én test brukerkonto med en av de riktige lisensene.</span><span class="sxs-lookup"><span data-stu-id="d6610-110">You have at least one administrator account and one test user account with one of the appropriate license.</span></span>
- <span data-ttu-id="d6610-111">Du må koble Azure AD Connect til den primære domenekontroller-emulatoren for at tilbakeskriving av passord skal fungere.</span><span class="sxs-lookup"><span data-stu-id="d6610-111">You must connect Azure AD Connect to the Primary Domain Controller Emulator for password writeback to work.</span></span> <span data-ttu-id="d6610-112">Du kan konfigurere Azure AD Connect til å bruke  en primær domenekontroller ved å høyreklikke på egenskapene for Active Directory-synkroniseringskontakten og deretter velge **Konfigurer katalogpartisjoner.**</span><span class="sxs-lookup"><span data-stu-id="d6610-112">You can configure Azure AD Connect to use a Primary Domain Controller by right clicking on the **properties** of the Active Directory synchronization connector, then selecting **configure directory partitions**.</span></span> <span data-ttu-id="d6610-113">Derfra kan du se etter **delen** for tilkoblingsinnstillinger for domenekontrolleren, og merke av i boksen med tittelen Bare **bruke foretrukne domenekontrollere.**</span><span class="sxs-lookup"><span data-stu-id="d6610-113">From there, look for the **domain controller connection settings** section and check the box titled **only use preferred domain controllers**.</span></span>
  > [!NOTE]
  > <span data-ttu-id="d6610-114">Hvis den foretrukne DC ikke er en PDC-emulator, vil Azure AD Connect fortsatt ta kontakt med PDC for tilbakeskriving av passord.</span><span class="sxs-lookup"><span data-stu-id="d6610-114">If the preferred DC is not a PDC emulator, Azure AD Connect will still reach out to the PDC for password writeback.</span></span>
- <span data-ttu-id="d6610-115">Tilbakestilling av passord er konfigurert og aktivert i tenanten din.</span><span class="sxs-lookup"><span data-stu-id="d6610-115">Password reset has been configured and enabled in your tenant.</span></span> <span data-ttu-id="d6610-116">Hvis du vil ha mer informasjon, kan du [se Aktivere brukere til å tilbakestille Azure AD-passordene sine.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)</span><span class="sxs-lookup"><span data-stu-id="d6610-116">For more information, see [Enable users to reset their Azure AD passwords](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span></span>
- <span data-ttu-id="d6610-117">Kontroller at administratorkontoen som brukes til å aktivere passordskriving, er en administratorkonto i skyen (opprettet i Azure AD, ikke lokalt AD)</span><span class="sxs-lookup"><span data-stu-id="d6610-117">Make sure that the administrator account being used to enable Password Writeback is a cloud administrator account (created in Azure AD not on-premises AD)</span></span>
- <span data-ttu-id="d6610-118">Du har en AD-distribusjon med én eller flere skoger lokalt som kjører Windows Server 2008 R2, Windows Server 2012 eller Windows Server 2012 R2 med de nyeste oppdateringspakkene installert</span><span class="sxs-lookup"><span data-stu-id="d6610-118">You have a single or multi-forest AD on-premises deployment running Windows Server 2008 R2, Windows Server 2012, or Windows Server 2012 R2 with the latest service packs installed</span></span>
- <span data-ttu-id="d6610-119">Du har Azure AD Connect-verktøyet installert, og du har klargjort AD-miljøet for synkronisering til skyen.</span><span class="sxs-lookup"><span data-stu-id="d6610-119">You have the Azure AD Connect tool installed and you have prepared your AD environment for synchronization to the cloud.</span></span> <span data-ttu-id="d6610-120">Før du tester tilbakeskriving av passord, må du først fullføre en fullstendig import og full synkronisering fra både AD og Azure AD i Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="d6610-120">Before testing password writeback, make sure that you first complete a full import and full sync from both AD and Azure AD in Azure AD Connect.</span></span>
- <span data-ttu-id="d6610-121">Hvis du vil ha mer informasjon, kan du se hvordan du gjør en fullstendig synkronisering [og full import i Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span><span class="sxs-lookup"><span data-stu-id="d6610-121">To learn more, see how to do a [full sync and full import in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span></span>

<span data-ttu-id="d6610-122">**Jeg har et problem med tilkobling med tilbakeskriving av passord**</span><span class="sxs-lookup"><span data-stu-id="d6610-122">**I'm having a problem with password writeback connectivity**</span></span>

1. <span data-ttu-id="d6610-123">Laste ned og aktivere den nyeste versjonen av [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span><span class="sxs-lookup"><span data-stu-id="d6610-123">Download and enable the latest version of [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span></span>
2. <span data-ttu-id="d6610-124">Brannmurkonfigurasjon: Azure AD Connect-verktøyet (1.1.443 og nyere) trenger **utgående HTTPS-tilgang** til:</span><span class="sxs-lookup"><span data-stu-id="d6610-124">Firewall configuration: The Azure AD Connect tool (1.1.443 and above) will need **outbound HTTPS** access to:</span></span>
    - <span data-ttu-id="d6610-125">passwordreset.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="d6610-125">passwordreset.microsoftonline.com</span></span>
    - <span data-ttu-id="d6610-126">servicebus.windows.networks</span><span class="sxs-lookup"><span data-stu-id="d6610-126">servicebus.windows.networks</span></span>
3. <span data-ttu-id="d6610-127">Tillat inaktive tilkoblinger å beholde i minst 2–3 minutter</span><span class="sxs-lookup"><span data-stu-id="d6610-127">Allow idle connections to persist for at least 2-3 minutes</span></span>

<span data-ttu-id="d6610-128">**Jeg har fortsatt problemer med tilbakeskriving av passord**</span><span class="sxs-lookup"><span data-stu-id="d6610-128">**I'm still having problems with password writeback**</span></span>

- <span data-ttu-id="d6610-129">Hvis du fremdeles har problemer, kan du prøve å deaktivere og aktivere tilbakeskrivingstjenesten for passord på nytt i Azure AD Connect-verktøyet</span><span class="sxs-lookup"><span data-stu-id="d6610-129">If you are still having difficulty, try disabling and re-enabling the password writeback service in the Azure AD Connect tool</span></span>
- <span data-ttu-id="d6610-130">Hvis du vil ha mer informasjon, kan du se hvordan [du deaktiverer og aktiverer tilbakeskriving](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot) av passord på nytt</span><span class="sxs-lookup"><span data-stu-id="d6610-130">To learn more, see how to [disable and re-enable password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span></span>
