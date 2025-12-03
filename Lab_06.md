# Create a Topic in Copilot Studio to Create an employee using Adaptative Card

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

<img width="1124" height="556" alt="image" src="https://github.com/user-attachments/assets/f80b3b88-3a57-4f77-88ac-26b0dae15304" />



## Step 4: Add a Question Node Show a message

1. Click the **+** button below the trigger node
2. Select **Ask a question**
3. Configure the Node:
   - Put the question: **Do you want to create a new employee:**
4. Indentify: Select **Boolean**
5. Create a condition

<img width="900" height="514" alt="image" src="https://github.com/user-attachments/assets/5b85aa0a-0b5c-4a93-91c0-35748df34066" />

## Step 5: Create a node to ask for the data with adaptive Card

1. Click the **+** button below your question node
2. Select **Ask with adaptive card**

<img width="556" height="415" alt="image" src="https://github.com/user-attachments/assets/dabcb173-3d30-4d98-8202-95c9c174049a" />

## Step 6: Create the json file for the adaptive card

1. Use Copilot to create the json
   Could you create an adatative card with Name, Surname, and Level. The level must be Level1 or Level2

   You receive some similar to this:
```
   {
  "$schema": "http://adaptivecards.io/schemas/adaptive-card.json",
  "type": "AdaptiveCard",
  "version": "1.4",
  "body": [
    {
      "type": "Input.Text",
      "id": "name",
      "label": "Name",
      "isRequired": true,
      "errorMessage": "Please enter a name."
    },
    {
      "type": "Input.Text",
      "id": "surname",
      "label": "Surname",
      "isRequired": true,
      "errorMessage": "Please enter a surname."
    },
    {
      "type": "Input.ChoiceSet",
      "id": "level",
      "label": "Level",
      "style": "compact",
      "choices": [
        { "title": "Level1", "value": "Level1" },
        { "title": "Level2", "value": "Level2" }
      ]
    }
  ],
  "actions": [
    {
      "type": "Action.Submit",
      "title": "Submit"
    }
  ]
}

```
## Step 7: Create the json file for the adaptive card

<img width="1015" height="591" alt="image" src="https://github.com/user-attachments/assets/cee7e620-3c86-472e-a17f-0913e4b1d73c" />

Copy you json in the editor:

<img width="1700" height="747" alt="image" src="https://github.com/user-attachments/assets/712a4343-7b4f-4165-a19f-ebe8b3e4fa3c" />


Close the **adaptive card editor**

## Step 8: Create a node to ask for the data

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
   - "I need to create a new employee in Business Central"
  
```
4. Verify:
   - Topic triggers correctly
   - Flow executes and returns data
   - Customer information displays properly
   - Error handling works for non-existent customers
