# Create a Topic in Copilot Studio to Read Companies from Business Central

## Prerequisites

- Access to Microsoft Copilot Studio
- Microsoft Dynamics 365 Business Central environment
- Business Central connector permissions
- Admin or maker role in Copilot Studio

## Overview

This guide will help you create a topic that allows your Copilot agent to retrieve and display the customer list from Business Central.

---

## Step 1: Access Your Agent in Copilot Studio

1. Navigate to [Microsoft Copilot Studio](https://copilotstudio.microsoft.com)
2. Sign in with your credentials
3. Select your agent or create a new one
4. Click on **Tools** in the left navigation panel

## Step 2: Create a New Tool

1. Click **Add Tool** 
2. Filter by **Connector**
3. Search for: `Companies`
4. Choose **List companies (V3)**

   <img width="596" height="371" alt="image" src="https://github.com/user-attachments/assets/7964f9e0-15f6-464a-a6e9-985016aeec93" />


## Step 3: Configure tool

Please don't configure any value here.

Click **Save**


<img width="1110" height="636" alt="image" src="https://github.com/user-attachments/assets/c1e1d2f6-1f24-4a3f-b018-a7e84e2f667a" />



## Step 4: Test Your Connector

1. Click **Test** to open the test pane
2. Try this prompt:
```
   - Could you give me the companies from Business Central?
  
```
3. Verify:
   - The connector triggers correctly

---

**Congratulations!** You've successfully created a topic that reads customer data from Business Central and displays it conversationally in your Copilot agent.

R.Corella

v. 1.0   December 2025
