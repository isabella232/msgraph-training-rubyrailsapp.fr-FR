<!-- markdownlint-disable MD002 MD041 -->

<span data-ttu-id="e1aea-101">Dans cet exercice, vous allez créer une inscription de l’application Web Azure AD à l’aide du centre d’administration Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e1aea-101">In this exercise, you will create a new Azure AD web application registration using the Azure Active Directory admin center.</span></span>

1. <span data-ttu-id="e1aea-102">Ouvrez un navigateur et accédez au [Centre d’administration Azure Active Directory](https://aad.portal.azure.com).</span><span class="sxs-lookup"><span data-stu-id="e1aea-102">Open a browser and navigate to the [Azure Active Directory admin center](https://aad.portal.azure.com).</span></span> <span data-ttu-id="e1aea-103">Connectez-vous à l’aide d’un **compte personnel** (compte Microsoft) ou d’un **compte professionnel ou scolaire**.</span><span class="sxs-lookup"><span data-stu-id="e1aea-103">Login using a **personal account** (aka: Microsoft Account) or **Work or School Account**.</span></span>

1. <span data-ttu-id="e1aea-104">Sélectionnez **Azure Active Directory** dans le volet de navigation de gauche, puis sélectionnez **inscriptions des applications** sous **gérer**.</span><span class="sxs-lookup"><span data-stu-id="e1aea-104">Select **Azure Active Directory** in the left-hand navigation, then select **App registrations** under **Manage**.</span></span>

    ![<span data-ttu-id="e1aea-105">Capture d’écran des inscriptions d’application</span><span class="sxs-lookup"><span data-stu-id="e1aea-105">A screenshot of the App registrations</span></span> ](./images/aad-portal-app-registrations.png)

1. <span data-ttu-id="e1aea-106">Sélectionnez **Nouvelle inscription**.</span><span class="sxs-lookup"><span data-stu-id="e1aea-106">Select **New registration**.</span></span> <span data-ttu-id="e1aea-107">Sur la page **Inscrire une application**, définissez les valeurs comme suit.</span><span class="sxs-lookup"><span data-stu-id="e1aea-107">On the **Register an application** page, set the values as follows.</span></span>

    - <span data-ttu-id="e1aea-108">Définissez le **Nom** sur `Ruby Graph Tutorial`.</span><span class="sxs-lookup"><span data-stu-id="e1aea-108">Set **Name** to `Ruby Graph Tutorial`.</span></span>
    - <span data-ttu-id="e1aea-109">Définissez les **Types de comptes pris en charge** sur **Comptes dans un annuaire organisationnel et comptes personnels Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="e1aea-109">Set **Supported account types** to **Accounts in any organizational directory and personal Microsoft accounts**.</span></span>
    - <span data-ttu-id="e1aea-110">Sous **URI de redirection**, définissez la première flèche déroulante sur `Web`, et la valeur sur `http://localhost:3000/auth/microsoft_graph_auth/callback`.</span><span class="sxs-lookup"><span data-stu-id="e1aea-110">Under **Redirect URI**, set the first drop-down to `Web` and set the value to `http://localhost:3000/auth/microsoft_graph_auth/callback`.</span></span>

    ![Capture d’écran de la page inscrire une application](./images/aad-register-an-app.png)

1. <span data-ttu-id="e1aea-112">Sélectionnez **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="e1aea-112">Select **Register**.</span></span> <span data-ttu-id="e1aea-113">Sur la page du **didacticiel Ruby Graph** , copiez la valeur de l' **ID d’application (client)** et enregistrez-la, vous en aurez besoin à l’étape suivante.</span><span class="sxs-lookup"><span data-stu-id="e1aea-113">On the **Ruby Graph Tutorial** page, copy the value of the **Application (client) ID** and save it, you will need it in the next step.</span></span>

    ![Capture d’écran de l’ID d’application de la nouvelle inscription de l’application](./images/aad-application-id.png)

1. <span data-ttu-id="e1aea-115">Sélectionnez **Certificats et secrets** sous **Gérer**.</span><span class="sxs-lookup"><span data-stu-id="e1aea-115">Select **Certificates & secrets** under **Manage**.</span></span> <span data-ttu-id="e1aea-116">Sélectionnez le bouton **Nouveau secret client**.</span><span class="sxs-lookup"><span data-stu-id="e1aea-116">Select the **New client secret** button.</span></span> <span data-ttu-id="e1aea-117">Entrez une valeur dans **Description** et sélectionnez l’une des options pour \*\*\*\* expirer, puis sélectionnez **Ajouter**.</span><span class="sxs-lookup"><span data-stu-id="e1aea-117">Enter a value in **Description** and select one of the options for **Expires** and select **Add**.</span></span>

    ![Capture d’écran de la boîte de dialogue Ajouter une clé secrète client](./images/aad-new-client-secret.png)

1. <span data-ttu-id="e1aea-119">Copiez la valeur du secret client avant de quitter cette page.</span><span class="sxs-lookup"><span data-stu-id="e1aea-119">Copy the client secret value before you leave this page.</span></span> <span data-ttu-id="e1aea-120">Vous en aurez besoin à l’étape suivante.</span><span class="sxs-lookup"><span data-stu-id="e1aea-120">You will need it in the next step.</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="e1aea-121">Ce secret client n’apparaîtra plus jamais, aussi veillez à le copier maintenant.</span><span class="sxs-lookup"><span data-stu-id="e1aea-121">This client secret is never shown again, so make sure you copy it now.</span></span>

    ![Capture d’écran de la clé secrète client récemment ajoutée](./images/aad-copy-client-secret.png)
