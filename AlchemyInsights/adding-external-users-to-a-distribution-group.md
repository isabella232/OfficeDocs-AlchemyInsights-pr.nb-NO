---
title: Legge til eksterne brukere i en distribusjons gruppe
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663522"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="1557b-102">Legge til eksterne brukere i en distribusjons gruppe</span><span class="sxs-lookup"><span data-stu-id="1557b-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="1557b-103">Å legge til en ekstern kontakt i en distribusjons gruppe (DG) er en to trinns prosess:</span><span class="sxs-lookup"><span data-stu-id="1557b-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="1557b-104">Opprette en e-postkontakt for den eksterne brukeren:</span><span class="sxs-lookup"><span data-stu-id="1557b-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="1557b-105">Gå til **brukerens**  >  [kontakter](https://admin.microsoft.com/adminportal/home#/Contact) -side i administrasjons senteret.</span><span class="sxs-lookup"><span data-stu-id="1557b-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="1557b-106">Velg **Legg til en kontakt**.</span><span class="sxs-lookup"><span data-stu-id="1557b-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="1557b-107">Skriv inn informasjonen for kontakten, og velg **Legg til**.</span><span class="sxs-lookup"><span data-stu-id="1557b-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="1557b-108">Legg til e-postkontakten i DG:</span><span class="sxs-lookup"><span data-stu-id="1557b-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="1557b-109">Gå til **grupper**  >  [grupper](https://admin.microsoft.com/adminportal/home#/groups) -siden i administrasjons senteret.</span><span class="sxs-lookup"><span data-stu-id="1557b-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="1557b-110">Finn DG du vil legge til den eksterne brukeren i, og velg den for å åpne dialog boksen Rediger.</span><span class="sxs-lookup"><span data-stu-id="1557b-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="1557b-111">Velg **Vis alle og behandle medlemmer**på fanen **medlemmer** .</span><span class="sxs-lookup"><span data-stu-id="1557b-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="1557b-112">Velg **Legg til medlemmer**.</span><span class="sxs-lookup"><span data-stu-id="1557b-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="1557b-113">Velg e-postkontakten du opprettet i forrige trinn, og velg deretter **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="1557b-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="1557b-114">Hvis de eksterne brukerne ikke kan sende e-postmeldinger til DG eller ikke motta e-postmeldinger fra det, kan det være at DG er merket for bare å tillate e-postmeldinger fra interne brukere.</span><span class="sxs-lookup"><span data-stu-id="1557b-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="1557b-115">Du kan kontrollere denne konfigurasjonen og rette den ved å følge instruksjonene [her](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="1557b-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="1557b-116">**Obs!** Disse instruksjonene gjelder ikke hvis gruppens type er Microsoft 365 Group i stedet for "distribusjons gruppe".</span><span class="sxs-lookup"><span data-stu-id="1557b-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="1557b-117">Hvis det er tilfelle, kan du legge til den eksterne brukeren direkte i gruppen fra Outlook.</span><span class="sxs-lookup"><span data-stu-id="1557b-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="1557b-118">Detaljert informasjon om Microsoft 365 grupper gjester samt instruksjoner for hvordan du legger til eksterne gjester, finner du i [denne artikkelen](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="1557b-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  