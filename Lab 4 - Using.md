# Create a Topic in Copilot Studio to create an Employee in Business Central

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
4. Click on **Topics** in the left navigation panel

## Step 2: Create a New Topic

1. Click **+ Add a topic** or **+ New topic**
2. Select **From blank**
3. Name your topic: `Create a new employee`
4. Add a description: `Create new employee in Business Central`

   

## Step 3: Configure Topic Trigger Phrases

Add trigger phrases that will activate this topic:

1. In the **Trigger** section, click **Edit**
2. Add the following description:
```
  I want to create an employee in Business Central
```
3. Click **Save**

<img width="468" height="279" alt="image" src="https://github.com/user-attachments/assets/66170016-05f6-40c8-a1a9-ce2093d055c5" />


## Step 4: Add a Question Node Show a message

1. Click the **+** button below the trigger node
2. Select **Ask a question**
3. Configure the Node:
   - Put the question: **Could you give me the employee name:**
4. Indentify: Select **User's entire response**
5. Change the variable name: varName

<img width="488" height="366" alt="image" src="https://github.com/user-attachments/assets/8ce31baf-ec75-494a-bd2d-46bca0422edb" />


## Step 5: Create a node to add a Tool

1. Click the **+** button below your question node
2. Select **Add a Tool**
3. Click **Basic Tools**
4. Click **New Agent Flow**

<img width="789" height="697" alt="image" src="https://github.com/user-attachments/assets/b86711d2-0936-4689-92a8-6d4929dfcf81" />



4. Create an **Agent Flow** (Power Automate)

   <img width="936" height="571" alt="image" src="https://github.com/user-attachments/assets/e2f90469-1fd8-410d-9c29-1ac3a51f653d" />

   Use the action **Create record (V3)**

   <img width="790" height="614" alt="image" src="https://github.com/user-attachments/assets/15c913ff-ce43-4df7-9512-3d388a8fb624" />
   
   Obtain the response to Copilot Studio:

   <img width="800" height="200" alt="image" src="https://github.com/user-attachments/assets/cd1f79e2-7466-4598-ba31-f52cd747f441" />


## Step 6: Show the Employee No. result adding other message with the variable.

<img width="559" height="472" alt="image" src="https://github.com/user-attachments/assets/5e458430-cc1b-42dd-b392-94adf48c29b7" />



## Step 7: Test Your Topic

1. Click **Save** in the top right
2. Click **Test** to open the test pane
3. Try trigger phrases:
```
   - "I need create a new employee in Business Central"
  
```
4. Verify:
   - Topic triggers correctly
   - Flow executes and returns data
   - Customer information displays properly
   - Error handling works for non-existent customers
