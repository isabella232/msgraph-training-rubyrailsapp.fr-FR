# <a name="how-to-run-the-completed-project"></a><span data-ttu-id="4f0d9-101">Exécution du projet terminé</span><span class="sxs-lookup"><span data-stu-id="4f0d9-101">How to run the completed project</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f0d9-102">Conditions préalables</span><span class="sxs-lookup"><span data-stu-id="4f0d9-102">Prerequisites</span></span>

<span data-ttu-id="4f0d9-103">Pour exécuter le projet terminé dans ce dossier, vous avez besoin des éléments suivants:</span><span class="sxs-lookup"><span data-stu-id="4f0d9-103">To run the completed project in this folder, you need the following:</span></span>

- <span data-ttu-id="4f0d9-104">[Ruby](https://www.ruby-lang.org/en/downloads/) est installé sur votre ordinateur de développement.</span><span class="sxs-lookup"><span data-stu-id="4f0d9-104">[Ruby](https://www.ruby-lang.org/en/downloads/) installed on your development machine.</span></span> <span data-ttu-id="4f0d9-105">Si vous n'avez pas Ruby, visitez le lien précédent pour obtenir les options de téléchargement.</span><span class="sxs-lookup"><span data-stu-id="4f0d9-105">If you do not have Ruby, visit the previous link for download options.</span></span> <span data-ttu-id="4f0d9-106">(**Remarque:** ce didacticiel a été écrit avec Ruby version 2.4.4.</span><span class="sxs-lookup"><span data-stu-id="4f0d9-106">(**Note:** This tutorial was written with Ruby version 2.4.4.</span></span> <span data-ttu-id="4f0d9-107">Les étapes de ce guide peuvent fonctionner avec d'autres versions, mais cela n'a pas été testé.)</span><span class="sxs-lookup"><span data-stu-id="4f0d9-107">The steps in this guide may work with other versions, but that has not been tested.)</span></span>
- <span data-ttu-id="4f0d9-108">Soit un compte Microsoft personnel avec une boîte aux lettres sur Outlook.com, soit un compte professionnel ou scolaire Microsoft.</span><span class="sxs-lookup"><span data-stu-id="4f0d9-108">Either a personal Microsoft account with a mailbox on Outlook.com, or a Microsoft work or school account.</span></span>

<span data-ttu-id="4f0d9-109">Si vous n'avez pas de compte Microsoft, vous disposez de deux options pour obtenir un compte gratuit:</span><span class="sxs-lookup"><span data-stu-id="4f0d9-109">If you don't have a Microsoft account, there are a couple of options to get a free account:</span></span>

- <span data-ttu-id="4f0d9-110">Vous pouvez vous [inscrire pour obtenir un nouveau compte Microsoft personnel](https://signup.live.com/signup?wa=wsignin1.0&rpsnv=12&ct=1454618383&rver=6.4.6456.0&wp=MBI_SSL_SHARED&wreply=https://mail.live.com/default.aspx&id=64855&cbcxt=mai&bk=1454618383&uiflavor=web&uaid=b213a65b4fdc484382b6622b3ecaa547&mkt=E-US&lc=1033&lic=1).</span><span class="sxs-lookup"><span data-stu-id="4f0d9-110">You can [sign up for a new personal Microsoft account](https://signup.live.com/signup?wa=wsignin1.0&rpsnv=12&ct=1454618383&rver=6.4.6456.0&wp=MBI_SSL_SHARED&wreply=https://mail.live.com/default.aspx&id=64855&cbcxt=mai&bk=1454618383&uiflavor=web&uaid=b213a65b4fdc484382b6622b3ecaa547&mkt=E-US&lc=1033&lic=1).</span></span>
- <span data-ttu-id="4f0d9-111">Vous pouvez vous [inscrire au programme pour les développeurs office 365](https://developer.microsoft.com/office/dev-program) pour obtenir un abonnement gratuit à Office 365.</span><span class="sxs-lookup"><span data-stu-id="4f0d9-111">You can [sign up for the Office 365 Developer Program](https://developer.microsoft.com/office/dev-program) to get a free Office 365 subscription.</span></span>

## <a name="register-a-web-application-with-the-azure-active-directory-admin-center"></a><span data-ttu-id="4f0d9-112">Enregistrer une application Web avec le centre d'administration Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="4f0d9-112">Register a web application with the Azure Active Directory admin center</span></span>

1. <span data-ttu-id="4f0d9-113">Ouvrez un navigateur et accédez au [Centre d'administration Azure Active Directory](https://aad.portal.azure.com).</span><span class="sxs-lookup"><span data-stu-id="4f0d9-113">Open a browser and navigate to the [Azure Active Directory admin center](https://aad.portal.azure.com).</span></span> <span data-ttu-id="4f0d9-114">Connectez-vous à l'aide d'un compte **personnel** (alias Microsoft) ou **compte professionnel ou scolaire**.</span><span class="sxs-lookup"><span data-stu-id="4f0d9-114">Login using a **personal account** (aka: Microsoft Account) or **Work or School Account**.</span></span>

1. <span data-ttu-id="4f0d9-115">Sélectionnez **Azure Active Directory** dans le volet de navigation de gauche, puis sélectionnez **inscriptions des applications (aperçu)** sous **gérer**.</span><span class="sxs-lookup"><span data-stu-id="4f0d9-115">Select **Azure Active Directory** in the left-hand navigation, then select **App registrations (Preview)** under **Manage**.</span></span>

    ![<span data-ttu-id="4f0d9-116">Capture d'écran des inscriptions d'application</span><span class="sxs-lookup"><span data-stu-id="4f0d9-116">A screenshot of the App registrations</span></span> ](/tutorial/images/aad-portal-app-registrations.png)

1. <span data-ttu-id="4f0d9-117">Sélectionnez **nouvelle inscription**.</span><span class="sxs-lookup"><span data-stu-id="4f0d9-117">Select **New registration**.</span></span> <span data-ttu-id="4f0d9-118">Sur la page **inscrire une application** , définissez les valeurs comme suit.</span><span class="sxs-lookup"><span data-stu-id="4f0d9-118">On the **Register an application** page, set the values as follows.</span></span>

    - <span data-ttu-id="4f0d9-119">Définissez **nom** sur `Ruby Graph Tutorial`.</span><span class="sxs-lookup"><span data-stu-id="4f0d9-119">Set **Name** to `Ruby Graph Tutorial`.</span></span>
    - <span data-ttu-id="4f0d9-120">Définissez les types de comptes **pris en charge** sur **les comptes de tous les comptes d'annuaire et de Microsoft personnels**.</span><span class="sxs-lookup"><span data-stu-id="4f0d9-120">Set **Supported account types** to **Accounts in any organizational directory and personal Microsoft accounts**.</span></span>
    - <span data-ttu-id="4f0d9-121">Sous **URI**de redirection, définissez la première liste déroulante sur `Web` et définissez la `http://localhost:3000/auth/microsoft_graph_auth/callback`valeur sur.</span><span class="sxs-lookup"><span data-stu-id="4f0d9-121">Under **Redirect URI**, set the first drop-down to `Web` and set the value to `http://localhost:3000/auth/microsoft_graph_auth/callback`.</span></span>

    ![Capture d'écran de la page inscrire une application](/tutorial/images/aad-register-an-app.png)

1. <span data-ttu-id="4f0d9-123">Sélectionnez **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="4f0d9-123">Choose **Register**.</span></span> <span data-ttu-id="4f0d9-124">Sur la page du **didacticiel Ruby Graph** , copiez la valeur de l' **ID d'application (client)** et enregistrez-la, vous en aurez besoin à l'étape suivante.</span><span class="sxs-lookup"><span data-stu-id="4f0d9-124">On the **Ruby Graph Tutorial** page, copy the value of the **Application (client) ID** and save it, you will need it in the next step.</span></span>

    ![Capture d'écran de l'ID d'application de la nouvelle inscription de l'application](/tutorial/images/aad-application-id.png)

1. <span data-ttu-id="4f0d9-126">Sélectionnez **certificats & secrets** sous **gérer**.</span><span class="sxs-lookup"><span data-stu-id="4f0d9-126">Select **Certificates & secrets** under **Manage**.</span></span> <span data-ttu-id="4f0d9-127">Sélectionnez le bouton **nouveau client secrète** .</span><span class="sxs-lookup"><span data-stu-id="4f0d9-127">Select the **New client secret** button.</span></span> <span data-ttu-id="4f0d9-128">Entrez une valeur dans **Description** , puis sélectionnez l'une des options \*\*\*\* pour expirer, puis choisissez **Ajouter**.</span><span class="sxs-lookup"><span data-stu-id="4f0d9-128">Enter a value in **Description** and select one of the options for **Expires** and choose **Add**.</span></span>

    ![Capture d'écran de la boîte de dialogue Ajouter une clé secrète client](/tutorial/images/aad-new-client-secret.png)

1. <span data-ttu-id="4f0d9-130">Copiez la valeur de la clé secrète client avant de quitter cette page.</span><span class="sxs-lookup"><span data-stu-id="4f0d9-130">Copy the client secret value before you leave this page.</span></span> <span data-ttu-id="4f0d9-131">Vous en aurez besoin à l'étape suivante.</span><span class="sxs-lookup"><span data-stu-id="4f0d9-131">You will need it in the next step.</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="4f0d9-132">Cette clé secrète client ne s'affiche plus, vérifiez que vous la copiez maintenant.</span><span class="sxs-lookup"><span data-stu-id="4f0d9-132">This client secret is never shown again, so make sure you copy it now.</span></span>

    ![Capture d'écran de la clé secrète client récemment ajoutée](/tutorial/images/aad-copy-client-secret.png)

## <a name="configure-the-sample"></a><span data-ttu-id="4f0d9-134">Configurer l'exemple</span><span class="sxs-lookup"><span data-stu-id="4f0d9-134">Configure the sample</span></span>

1. <span data-ttu-id="4f0d9-135">Renommez `./config/oauth_environment_variables.rb.example` le fichier `oauth_environment_variables.rb`.</span><span class="sxs-lookup"><span data-stu-id="4f0d9-135">Rename the `./config/oauth_environment_variables.rb.example` file to `oauth_environment_variables.rb`.</span></span>
1. <span data-ttu-id="4f0d9-136">Modifiez le `oauth_environment_variables.rb` fichier et effectuez les modifications suivantes.</span><span class="sxs-lookup"><span data-stu-id="4f0d9-136">Edit the `oauth_environment_variables.rb` file and make the following changes.</span></span>
    1. <span data-ttu-id="4f0d9-137">Remplacez `YOUR_APP_ID_HERE` par l' **ID d'application** que vous avez obtenu à partir du portail d'inscription des applications.</span><span class="sxs-lookup"><span data-stu-id="4f0d9-137">Replace `YOUR_APP_ID_HERE` with the **Application Id** you got from the App Registration Portal.</span></span>
    1. <span data-ttu-id="4f0d9-138">Remplacez `YOUR APP PASSWORD HERE` par le mot de passe que vous avez obtenu à partir du portail d'inscription des applications.</span><span class="sxs-lookup"><span data-stu-id="4f0d9-138">Replace `YOUR APP PASSWORD HERE` with the password you got from the App Registration Portal.</span></span>
1. <span data-ttu-id="4f0d9-139">Dans votre interface de ligne de commande (CLI), accédez à ce répertoire et exécutez la commande suivante pour installer les conditions requises.</span><span class="sxs-lookup"><span data-stu-id="4f0d9-139">In your command-line interface (CLI), navigate to this directory and run the following command to install requirements.</span></span>

    ```Shell
    bundle install
    ```

1. <span data-ttu-id="4f0d9-140">Dans votre interface CLI, exécutez la commande suivante pour initialiser la base de données de l'application.</span><span class="sxs-lookup"><span data-stu-id="4f0d9-140">In your CLI, run the following command to initialize the app's database.</span></span>

    ```Shell
    rake db:migrate
    ```

## <a name="run-the-sample"></a><span data-ttu-id="4f0d9-141">Exécution de l’exemple</span><span class="sxs-lookup"><span data-stu-id="4f0d9-141">Run the sample</span></span>

1. <span data-ttu-id="4f0d9-142">Exécutez la commande suivante dans votre interface CLI pour démarrer l'application.</span><span class="sxs-lookup"><span data-stu-id="4f0d9-142">Run the following command in your CLI to start the application.</span></span>

    ```Shell
    rails server
    ```

1. <span data-ttu-id="4f0d9-143">Ouvrez un navigateur et accédez à `http://localhost:3000`.</span><span class="sxs-lookup"><span data-stu-id="4f0d9-143">Open a browser and browse to `http://localhost:3000`.</span></span>