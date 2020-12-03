---
title: Aktiver tilbakeskriving av passord i Azure AD Connect
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 0eecd89b2558359702935379d7ffbd8b7508f4cd
ms.sourcegitcommit: 62a83a1c6bd9779a1a11b749490bd11670d4b063
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/02/2020
ms.locfileid: "49560449"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="ed99b-102">Aktiver tilbakeskriving av passord i Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="ed99b-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="ed99b-103">Hvis du vil aktivere selvbetjent tilbakeskriving av passordtilbakestilling, må du først aktivere alternativet for tilbakeskriving i Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="ed99b-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="ed99b-104">Følg fremgangsmåten nedenfor fra Azure AD Connect-serveren din:</span><span class="sxs-lookup"><span data-stu-id="ed99b-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="ed99b-105">Logg på Azure AD Connect-påloggingsserveren, og start konfigurasjonsveiviseren for **Azure AD Connect**.</span><span class="sxs-lookup"><span data-stu-id="ed99b-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="ed99b-106">På **Velkommen**-siden klikker du på **Konfigurer**.</span><span class="sxs-lookup"><span data-stu-id="ed99b-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="ed99b-107">Velg **Tilpass synkroniseringsalternativer** på siden **Flere oppgaver**, og klikk deretter på **Neste**.</span><span class="sxs-lookup"><span data-stu-id="ed99b-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="ed99b-108">Skriv inn global administratorlegitimasjon for Azure-leieren på siden **Koble til Azure AD**, og klikk deretter på **Neste**.</span><span class="sxs-lookup"><span data-stu-id="ed99b-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="ed99b-109">Klikk på **Neste** på **Koble til kataloger** og **domene/OU**-filtreringssider.</span><span class="sxs-lookup"><span data-stu-id="ed99b-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="ed99b-110">På siden **Valgfrie funksjoner** merker du av i boksen ved siden av **Tilbakeskriving av passord** og klikker på **Neste**.</span><span class="sxs-lookup"><span data-stu-id="ed99b-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="ed99b-111">På siden **Klar for konfigurasjon** klikker du på **Konfigurer** og venter til prosessen er ferdig.</span><span class="sxs-lookup"><span data-stu-id="ed99b-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="ed99b-112">Når du ser konfigurasjonen er ferdig, klikker du på **Avslutt**.</span><span class="sxs-lookup"><span data-stu-id="ed99b-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="ed99b-113">Med tilbakeskriving av passord aktivert i Azure AD Connect konfigurerer du Azure AD SSPR for tilbakeskriving.</span><span class="sxs-lookup"><span data-stu-id="ed99b-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="ed99b-114">Hvis du vil aktivere tilbakeskriving av passord i SSPR, kan du fullføre følgende trinn:</span><span class="sxs-lookup"><span data-stu-id="ed99b-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="ed99b-115">Logg deg på Azure-portalen ved hjelp av en global administratorkonto.</span><span class="sxs-lookup"><span data-stu-id="ed99b-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="ed99b-116">Søk etter og velg **Azure Active Directory**, klikk på **Tilbakestilling av passord**, og klikk deretter på **Lokal integrering**.</span><span class="sxs-lookup"><span data-stu-id="ed99b-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="ed99b-117">Angi alternativet for **Tilbakeskrive passord til den lokale katalogen?** til **Ja**.</span><span class="sxs-lookup"><span data-stu-id="ed99b-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="ed99b-118">Angi alternativet for **Tillat brukere å låse opp kontoene uten å tilbakestille passordet?** til **Ja**.</span><span class="sxs-lookup"><span data-stu-id="ed99b-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="ed99b-119">Når du er klar, klikker du på **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="ed99b-119">When ready, click **Save**.</span></span>

<span data-ttu-id="ed99b-120">Hvis du vil ha mer informasjon, kan du se [Aktivere tilbakeskriving for selvbetjent passordtilbakestilling i Azure Active Directory til et lokalt miljø](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="ed99b-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="ed99b-121">Når en administrator tilbakestiller en brukers passord i Azure Portal, er det slik at hvis den brukeren er i forbund eller passordhashsynkronisert, blir passordet skrevet tilbake til det lokale miljøet.</span><span class="sxs-lookup"><span data-stu-id="ed99b-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="ed99b-122">Denne funksjonaliteten støttes for øyeblikket ikke i administrasjonsportalen for Office.</span><span class="sxs-lookup"><span data-stu-id="ed99b-122">This functionality is currently not supported in the Office Admin portal.</span></span>