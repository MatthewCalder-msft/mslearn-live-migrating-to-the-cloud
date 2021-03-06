# Prepare for session 5: "Monitoring and scaling your applications in Azure"

In session four we added a centralized, cloud-based storage to VanArsdel's solution. Now that the project is fully running in the cloud, we want to make sure things are going well.

In this session, you will:

* Monitor your application against metrics

* Configure Alerts when your application hits certain thresholds

* Setup scaling rules for your application

To follow along with the session, we recommend to get the project into the state we had at the end of session four.

## The instructions and scripts provided in this document will:

1. Create an App Service Plan
2. Create an App Service
3. Deploy the app directly from Github into the App Service
4. Create a logical database server
5. Create an Azure SQL Database
6. Configure the App Service to connect to the database
7. Create an Azure Storage Account
8. Set up Azure Blob Storage
9. Configure the App Service to connect to Azure Storage

## Prepare your environment

- Fork our repository ([aka.ms/vanarsdelrepo](https://aka.ms/vanarsdelrepo)) if not already done ([fork now](https://github.com/MicrosoftDocs/mslearn-live-migrating-to-the-cloud/fork))
- Clone the repository to your PC
- Open the completed solution under "src/2 - Completed" (you can use Visual Studio 2019 or Visual Studio Code)

### If you are using your Azure subscription

- Open [Azure Portal](https://portal.azure.com) in your browser and select your subscription
- Open the Cloud Shell (the button is located at the very top, next to the notifications bell and looks like this: >_) and select to use a "Bash" shell.

### If you are using the Learn Live Sandbox

- Go to your [Learn Live Sandbox activation page](https://aka.ms/learnlivesandbox)
- Locate Azure Cloud Shell on the right-hand side

Copy the following command and paste it into Cloud Shell:

`wget -O prepsession5.bash https://raw.githubusercontent.com/MicrosoftDocs/mslearn-live-migrating-to-the-cloud/master/scripts/03_deploy_app_service_and_database_and_storage.bash && chmod +x ./prepsession5.bash && ./prepsession5.bash`

**Note:** The script will prompt you to enter the URL of **your fork** of the Github repo. 

When finished, the script will output the URL of the App Service and append the query parameter `?forceMigration=true` - please follow this link to ensure the database gets populated with data.

You are now ready to join session five! :-)