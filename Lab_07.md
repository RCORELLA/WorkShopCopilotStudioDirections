# Create a Topic in Copilot Studio to manage employees onboarding

## Prerequisites

- Access to Microsoft Copilot Studio
- Microsoft Dynamics 365 Business Central environment
- Business Central connector permissions
- Admin or maker role in Copilot Studio

---

## Step 1: Access Your Agent in Copilot Studio

1. Navigate to [Microsoft Copilot Studio](https://copilotstudio.microsoft.com)
2. Sign in with your credentials
3. Select your agent or create a new one
4. Click on **Overview** and go to **Intructions**

## Step 2: Add instructions
```
  - Use Business Central MCP tool if you need to retrieve information from Business Central

  - If you need to create new employees, use the Topic Create new employees

  - The employees can review and order the new mobiles.  The list of devices depends on the statisticsGroupCode. Even if you don't have items available, show the list of items.

  - If the Statistics Group Code is LEVEL1 then the mobile availables, will be the list of items with Item Category code L1MOBILES

  - If the Statistics Group Code is LEVEL2 then the mobile availables will be the list of items with Item Category code L2MOBILES

```


## Step 3: Test Your Topic

1. Click **Save** in the top right
2. Click **Test** to open the test pane
3. Try trigger phrases:
```
   - "As employee, I need a new mobile. Could you give me the list of mobiles that I can buy?"

```

<img width="554" height="290" alt="image" src="https://github.com/user-attachments/assets/6958f4bb-442d-4c78-b60c-9ea65add229e" />

4. Verify:
   - Topic triggers correctly
   - Flow executes and returns data
   - Customer information displays properly
   - Error handling works for non-existent customers
