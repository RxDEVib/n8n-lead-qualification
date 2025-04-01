# Use case guide: Automating Lead-to-Deal Creation with n8n

Purpose:
This workflow automates the process of capturing new leads, creating deals, and notifying the sales team in real-time. Instead of manually entering lead details and updating the team, n8n ensures that all actions happen seamlessly with minimal human intervention.

Pain Points Addressed:

✅ Eliminates Manual Data Entry
- No more manual copying of lead details—reducing errors and saving time.

✅ Real-Time Team Collaboration

- Sales reps receive instant Slack notifications, allowing them to follow up quickly.

✅ Ensures Lead Tracking
- Every new lead is structured into HubSpot, ensuring no potential client is overlooked.

Why Use n8n for This?
- No-Code/Low-Code Flexibility – Easily customize workflows without deep coding knowledge.

-  Scalability – Can be expanded to include more CRM automation, follow-up reminders, or analytics tracking.

-   Seamless Integrations – Works smoothly with HubSpot, Slack, and other business tools.

This guide will walk you through the process of connecting n8n forms and creating a new contact in HubSpot CRM and sending a Slack notification. Follow the steps below for a seamless setup.

> **Note:** Before starting, ensure that n8n is set up locally on your machine or on the cloud. If not, complete the setup process as per the n8n documentation.

## Step 1: Understanding the Workflow
We will create a workflow similar to the one shown in the image below. 

![Workflow Diagram](\<Enter Insert Image Link/Path>)

## Step 2: Setting Up Authorization Tokens and Credentials
To connect HubSpot CRM and OpenAI, you'll need to generate API keys and tokens. Follow these steps:


## Step 3: Security Reminder
- Ensure all API tokens and keys are saved securely.
- Do **not** share your tokens in public forums or with unauthorized individuals.

## Step 4: Uploading the Workflow to n8n Cloud
1. Log in to your [n8n Cloud account](https://cloud.n8n.io/) OR visit your locally hosted n8n instance.[n8n local instance](http://localhost:5678)
2. Navigate to your dashboard.
3. Select **Workflows** → **Import from file**.
4. Upload the `<provide-file-name>.json` workflow file.
5. Confirm and run the workflow to verify the connection.

## Conclusion
You have now successfully connected n8n forms, HubSpot CRM and Slack using n8n. If you encounter any issues, refer to the respective documentation or contact support.

---

For further assistance, feel free to reach out to the support channels of HubSpot, or n8n.

Happy automating!