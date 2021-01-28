---
title: Logger og rapportering
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
- "9004331"
- "7727"
ms.openlocfilehash: 7349efb02f8d6ac5d73f6d6cd06eef6308ffe9be
ms.sourcegitcommit: 117c64e1fbcb5eec04f94eadad71423b974e7b14
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/27/2021
ms.locfileid: "50036007"
---
# <a name="logs-and-reporting"></a><span data-ttu-id="bf472-102">Logger og rapportering</span><span class="sxs-lookup"><span data-stu-id="bf472-102">Logs and Reporting</span></span>

<span data-ttu-id="bf472-103">[Vanlige spørsmål om Azure Active Directory-rapportering](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) svarer på vanlige spørsmål om Azure Active Directory-rapportering (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="bf472-103">[Azure Active Directory reporting FAQ](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) answers frequently asked questions about Azure Active Directory (Azure AD) reporting.</span></span> <span data-ttu-id="bf472-104">Hvis du vil ha mer informasjon, kan du [se rapportering for Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports)</span><span class="sxs-lookup"><span data-stu-id="bf472-104">For more information, see [Azure Active Directory reporting](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).</span></span>

<span data-ttu-id="bf472-105">**Feilsøke problemer med overvåking**</span><span class="sxs-lookup"><span data-stu-id="bf472-105">**Troubleshooting issues with Audit**</span></span>

1. <span data-ttu-id="bf472-106">Hvis du har problemer med å se noen overvåkingsaktiviteter og den manglende aktiviteten er i denne [listen,](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities)kan du sende inn en støtteforespørsel.</span><span class="sxs-lookup"><span data-stu-id="bf472-106">If you are having issues seeing some audit activities and the missing Activity is in this [list](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities), please file a support ticket.</span></span>
2. <span data-ttu-id="bf472-107">Hvis du har problemer med å se noen overvåkingslogger i tenanten din, kan du sende inn en støtteforespørsel.</span><span class="sxs-lookup"><span data-stu-id="bf472-107">If you are having issues seeing any Audit logs in your tenant, please file a support ticket.</span></span>
3. <span data-ttu-id="bf472-108">Hvis overvåkingsaktivitetene ikke vises umiddelbart i Azure [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) Portal, kan du sjekke ventetidsinformasjonen og arkivere en støtteforespørsel hvis forsinkelsen overskrider den dokumenterte ventetiden.</span><span class="sxs-lookup"><span data-stu-id="bf472-108">If your audit activities are not showing up immediately in the Azure Portal, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. [<span data-ttu-id="bf472-109">Oppbevaring av Azure AD-aktivitetslogger</span><span class="sxs-lookup"><span data-stu-id="bf472-109">Azure AD Activity Logs Retention</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. <span data-ttu-id="bf472-110">Hvis du ikke ser all overvåking av datoområdet du valgte, kan du laste ned opptil 250 000 rader (sortert etter siste) av pålogginger fra Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="bf472-110">If you don't see all the audit for the date range you selected, you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="bf472-111">Hvis du vil ha mer informasjon, kan du [se nedlasting av overvåkingsaktiviteter.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report)</span><span class="sxs-lookup"><span data-stu-id="bf472-111">For more information, see [Audit activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span></span>

<span data-ttu-id="bf472-112">**Feilsøke problemer med pålogginger**</span><span class="sxs-lookup"><span data-stu-id="bf472-112">**Troubleshooting issues with Sign-ins**</span></span>

1. <span data-ttu-id="bf472-113">Du kan bare se de siste 30 dagene med data hvis du har en Azure AD Premium-lisens (P1 eller P2) for leieren.</span><span class="sxs-lookup"><span data-stu-id="bf472-113">You can only see the last 30 days of data if you have an Azure AD Premium (P1 or P2) license for your tenant.</span></span>
2. <span data-ttu-id="bf472-114">Pålogginger er bare tilgjengelige for Azure AD Premium-tenanter.</span><span class="sxs-lookup"><span data-stu-id="bf472-114">Sign-ins are available only for Azure AD Premium tenants.</span></span> <span data-ttu-id="bf472-115">Den er ikke tilgjengelig for free- eller basic-lisensierte leiere.</span><span class="sxs-lookup"><span data-stu-id="bf472-115">It's not available for Free or Basic licensed tenants.</span></span>
3. <span data-ttu-id="bf472-116">Hvis leieren har en Premium P1-lisens og du ikke kan se [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) påloggingene, kan du se ventetidsinformasjonen vår og arkivere en støtteforespørsel hvis forsinkelsen overskrider den dokumenterte ventetiden.</span><span class="sxs-lookup"><span data-stu-id="bf472-116">If your tenant has a Premium P1 license and you can't see the sign-ins, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. <span data-ttu-id="bf472-117">Hvis du ikke ser alle påloggingene for datointervallet du valgte, kan du merke deg at du kan laste ned opptil 250 000 rader (sortert etter siste) av pålogginger fra Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="bf472-117">If you don't see all the sign-ins for the date range you selected, note that you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="bf472-118">Hvis du vil ha mer informasjon, kan du [se nedlasting av aktiviteter for pålogging.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities)</span><span class="sxs-lookup"><span data-stu-id="bf472-118">For more information, see [Sign-ins activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span></span>

<span data-ttu-id="bf472-119">**Feilsøke sikkerhetsrapporter (Brukere som er flagget ved risiko, risikabel pålogging)**</span><span class="sxs-lookup"><span data-stu-id="bf472-119">**Troubleshoot Security Reports (Users Flagged at Risk, Risky Sign-In)**</span></span>

1. [<span data-ttu-id="bf472-120">Brukere flagget for rapport om risikosikkerhet</span><span class="sxs-lookup"><span data-stu-id="bf472-120">Users flagged for risk security report</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [<span data-ttu-id="bf472-121">Rapport om risikabel pålogging i Azure Active Directory-portalen</span><span class="sxs-lookup"><span data-stu-id="bf472-121">Risky sign-ins report in the Azure Active Directory portal</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [<span data-ttu-id="bf472-122">Risikohendelser i Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="bf472-122">Azure Active Directory risk events</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
