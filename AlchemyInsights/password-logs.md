---
title: Passordlogger
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527176"
---
# <a name="password-logs"></a><span data-ttu-id="67cfb-102">Passordlogger</span><span class="sxs-lookup"><span data-stu-id="67cfb-102">Password logs</span></span>

<span data-ttu-id="67cfb-103">**Jeg har problemer med tilgang til overvåkingslogger for tilbakestilling av passord**</span><span class="sxs-lookup"><span data-stu-id="67cfb-103">**I'm having problems accessing password reset audit logs**</span></span>

<span data-ttu-id="67cfb-104">Utfør følgende trinn for å feilsøke problemer med tilgang til overvåkingslogger for tilbakestilling av passord:</span><span class="sxs-lookup"><span data-stu-id="67cfb-104">To troubleshoot issues regarding access to password reset audit logs, perform the following step:</span></span>

<span data-ttu-id="67cfb-105">Kontroller at du er autorisert til å vise overvåkingslogger.</span><span class="sxs-lookup"><span data-stu-id="67cfb-105">Ensure you are authorized to view audit logs.</span></span> 

<span data-ttu-id="67cfb-106">Bare følgende roller godkjennes:</span><span class="sxs-lookup"><span data-stu-id="67cfb-106">Only the following roles are authorized:</span></span>
 - <span data-ttu-id="67cfb-107">Global administrator</span><span class="sxs-lookup"><span data-stu-id="67cfb-107">Global administrator</span></span>
 - <span data-ttu-id="67cfb-108">Sikkerhetsadministrator</span><span class="sxs-lookup"><span data-stu-id="67cfb-108">Security administrator</span></span>
 - <span data-ttu-id="67cfb-109">Sikkerhetsleser</span><span class="sxs-lookup"><span data-stu-id="67cfb-109">Security reader</span></span>

<span data-ttu-id="67cfb-110">**Jeg vil se alle overvåkingshendelser for tilbakestilling av passord fra det tidspunktet da jeg opprinnelig distribuerte**</span><span class="sxs-lookup"><span data-stu-id="67cfb-110">**I want to see all password reset audit events from the time I initially deployed**</span></span>

<span data-ttu-id="67cfb-111">Opptil 120 000 hendelser for tilbakestilling/registrering av passord lagres i rapportene for de siste 30 dagene.</span><span class="sxs-lookup"><span data-stu-id="67cfb-111">Up to 120,000 password reset/registration events are stored in the reports of the last 30 days.</span></span> <span data-ttu-id="67cfb-112">Denne maksimumsgrensen gjelder for brukergrensesnittet når du laster ned CSV-filen.</span><span class="sxs-lookup"><span data-stu-id="67cfb-112">This maximum limit applies to the UI when downloading the CSV.</span></span> <span data-ttu-id="67cfb-113">1 million hendelser er tilgjengelige via PowerShell.</span><span class="sxs-lookup"><span data-stu-id="67cfb-113">1 million events are available through PowerShell.</span></span>
<span data-ttu-id="67cfb-114">Hvis du vil ha mer informasjon, kan du se koblingene nedenfor:</span><span class="sxs-lookup"><span data-stu-id="67cfb-114">For more information, see the links below:</span></span>

- [<span data-ttu-id="67cfb-115">Selvbetjente hendelser for tilbakestilling av passord fra API-rapporter og -hendelser for Azure AD</span><span class="sxs-lookup"><span data-stu-id="67cfb-115">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="67cfb-116">Slik laster du ned registreringshendelser for tilbakestilling av passord raskt med PowerShell</span><span class="sxs-lookup"><span data-stu-id="67cfb-116">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

<span data-ttu-id="67cfb-117">**Jeg ønsker å forstå mer om rapporteringsmuligheter for tilbakestilling av passord**</span><span class="sxs-lookup"><span data-stu-id="67cfb-117">**I want to understand more about password reset reporting capabilities**</span></span>

<span data-ttu-id="67cfb-118">Kontroller hvem som registrerer seg for eller tilbakestiller passord med overvåkingslogger for tilbakestilling av passord for Azure I Azure-portalen under **Brukere og grupper.**</span><span class="sxs-lookup"><span data-stu-id="67cfb-118">Check who is registering for or resetting passwords with Azure AD password reset audit logs in the Azure portal under **Users and groups**.</span></span>
<span data-ttu-id="67cfb-119">Hvis du vil ha mer informasjon, kan du se følgende koblinger:</span><span class="sxs-lookup"><span data-stu-id="67cfb-119">For more information, see the following links:</span></span>

- [<span data-ttu-id="67cfb-120">Oversikt over rapporter om tilbakestilling av passord</span><span class="sxs-lookup"><span data-stu-id="67cfb-120">Password reset reports overview</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="67cfb-121">Slik viser du rapporter for tilbakestilling av passord i Azure Portal</span><span class="sxs-lookup"><span data-stu-id="67cfb-121">How to view password reset reports in the Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="67cfb-122">Selvbetjente hendelser for tilbakestilling av passord fra API-rapporter og -hendelser for Azure AD</span><span class="sxs-lookup"><span data-stu-id="67cfb-122">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="67cfb-123">Slik laster du ned registreringshendelser for tilbakestilling av passord raskt med PowerShell</span><span class="sxs-lookup"><span data-stu-id="67cfb-123">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


