# Step-by-Step Guide: Connecting HubSpot CRM and Creating an Agentic Flow with OpenAI


This guide will walk you through the process of connecting HubSpot CRM and \<Add the tools required>. Follow the steps below for a seamless setup.

> **Note:** Before starting, ensure that n8n is set up locally on your machine or on the cloud. If not, complete the setup process as per the n8n documentation.

## Step 1: Understanding the Workflow
We will create a workflow similar to the one shown in the image below. 

![Workflow Diagram](\<Enter Insert Image Link/Path>)

## Step 2: Setting Up Authorization Tokens and Credentials
To connect HubSpot CRM and OpenAI, you'll need to generate API keys and tokens. Follow these steps:

### 2.2 Registering for HubSpot CRM
1. Visit the [HubSpot website](https://www.hubspot.com/) and sign up for an account.
2. Navigate to **Settings** → **Integrations** → **API Key**.
3. Generate a new API key.
4. Copy the key and store it safely.
> **Note:** If you are using n8n cloud. You can sign in to your HubSpot account and the credentials will be automatically saved.

## Step 3: Security Reminder
- Ensure all API tokens and keys are saved securely.
- Do **not** share your tokens in public forums or with unauthorized individuals.

## Step 4: Uploading the Workflow to n8n Cloud
1. Log in to your [n8n Cloud account](https://cloud.n8n.io/) OR visit your locally hosted n8n instance.[n8n local instance](http://localhost:5678)
2. Navigate to your dashboard.
3. Select **Workflows** → **Import from file**.
4. Upload the `<provide-file-name>.json` workflow file.
5. Confirm and run the workflow to verify the connection.


## Step 5: Configuring the HubSpot CRM Node (Local Instance)
1. Double-click on the **HubSpot CRM** node.
2. In the **Credential to connect with** field, select **+ Create new Credential**.
3. In connection, select **APP TOKEN**
4. Enter the **APP TOKEN** generated from HubSpot CRM earlier
5. Save it and close the window.

## Conclusion
You have now successfully connected HubSpot CRM and \<Add the tools required> using n8n. If you encounter any issues, refer to the respective documentation or contact support.

---

For further assistance, feel free to reach out to the support channels of HubSpot, or n8n.

Happy automating!
