# Create a Topic in Copilot Studio to Read Customers from Business Central

## Prerequisites

- Access to Microsoft Copilot Studio
- Microsoft Dynamics 365 Business Central environment
- Business Central connector permissions
- Admin or maker role in Copilot Studio

## Overview

This guide will help you create a topic that allows your Copilot agent to retrieve and display customer information from Business Central.

---

## Step 1: Access Your Agent in Copilot Studio

1. Navigate to [Microsoft Copilot Studio](https://copilotstudio.microsoft.com)
2. Sign in with your credentials
3. Select your agent or create a new one
4. Click on **Topics** in the left navigation panel

## Step 2: Create a New Topic

1. Click **+ Add a topic** or **+ New topic**
2. Select **From blank**
3. Name your topic: `Get Customer List`
4. Add a description: `Retrieves customers from Business Central`

## Step 3: Configure Topic Trigger Phrases

Add trigger phrases that will activate this topic:

1. In the **Trigger** section, click **Edit**
2. Add the following description:
```
  I want to obtain the Customer List from Business Central
```
3. Click **Save**
<img width="542" height="286" alt="image" src="https://github.com/user-attachments/assets/df5f73f9-61b3-46f5-8ecf-9fa8f399b9c4" />

## Step 4: Add a Question Node Show a message

1. Click the **+** button below the trigger node
2. Select **Send a message**
3. Configure the message:
   - **Nice I can help you with that**

## Step 5: Create a node to call an action

1. Click the **+** button below your question node
2. Select **Add a Tool**
3. Click **Conectors**

<img width="920" height="730" alt="image" src="https://github.com/user-attachments/assets/efabe245-dddb-44d0-9f1e-709909aa0f53" />

4. Fill the fields:
   
   <img width="586" height="629" alt="image" src="https://github.com/user-attachments/assets/6b4ef3ef-d9cb-4316-b8d0-6ded82f13d19" />


## Step 6: Show the result adding other message with the variable.

<img width="527" height="219" alt="image" src="https://github.com/user-attachments/assets/22e36763-84e5-4b46-a250-60b24486eb6a" />


## Step 7: Test Your Topic

1. Click **Save** in the top right
2. Click **Test** to open the test pane
3. Try trigger phrases:
```
   - "Show me customer List from Business Central"
  
```
4. Verify:
   - Topic triggers correctly
   - Flow executes and returns data
   - Customer information displays properly
   - Error handling works for non-existent customers


## Resources

- [Business Central API Documentation](https://learn.microsoft.com/dynamics365/business-central/dev-itpro/api-reference/v2.0/)
- [Power Automate Connectors](https://learn.microsoft.com/connectors/dynamicssmbsaas/)
- [Copilot Studio Topics Guide](https://learn.microsoft.com/microsoft-copilot-studio/authoring-create-edit-topics)

---

**Congratulations!** You've successfully created a topic that reads customer data from Business Central and displays it conversationally in your Copilot agent.
