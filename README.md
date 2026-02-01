**Dr. Strange Appointment Automation - n8n Webhook
Overview**

This n8n workflow automates the process of managing Dr. Strange appointments. Using a webhook, external applications or users can trigger the workflow to perform actions such as scheduling, notifications, or other automated tasks.

The workflow is designed for easy integration with other tools, allowing you to call it via a simple HTTP request.

<img width="470" height="194" alt="image" src="https://github.com/user-attachments/assets/661b387b-17fc-4c94-9086-f674e8406049" />


**Webhook URL**

You can trigger the workflow by sending a request to the following URL:

**Webhook URL:**
https://eshaan99999.app.n8n.cloud/webhook/a30fe26c-8b13-4c1e-82cb-22aa604b0ba1/chat

**How to Run**

**There are two ways to run this webhook:**

1. Test Mode

Open the workflow in the n8n editor.

Click Execute Workflow.

Immediately send a GET or POST request to the webhook URL.

GET request: Open the URL in a browser.

POST request: Send JSON data via Postman, curl, or any HTTP client.

The workflow executes once per execution in test mode.

**2. Active Mode (Recommended)**

Open the workflow in n8n.

Toggle the workflow to Active.

Once active, you can trigger the webhook any number of times using the URL.

**Example commands:**

GET request via browser:

Open https://eshaan99999.app.n8n.cloud/webhook/a30fe26c-8b13-4c1e-82cb-22aa604b0ba1/chat


**POST request via curl:**

curl -X POST "https://eshaan99999.app.n8n.cloud/webhook/a30fe26c-8b13-4c1e-82cb-22aa604b0ba1/chat" \
     -H "Content-Type: application/json" \
     -d '{"name":"Eshaan","time":"10:00 AM"}'

**Tools / Requirements**

n8n account: To edit, activate, or view the workflow.

HTTP client: Browser, Postman, curl, or any tool to send GET/POST requests.

JSON data (if using POST): Ensure the correct keys/values expected by the workflow.

**Notes

Ensure the workflow is active to allow repeated webhook calls.

In test mode, the webhook works only once per execution.

The workflow can be integrated into other applications for appointment scheduling automation.**
