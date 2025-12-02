# The Pocket Sales Assistant

**The Pain:** Salespeople on the road waste time calling the office to ask: “Do we have stock of this?” or “At what price should I sell this to the customer?”

**The Exercise:** Create an agent that retrieves real-time data from **Business Central**

**Flow:**
1. The user writes in Teams: “How many Berlin Chairs (Item 1900-S) do we have and what’s the price for Adatum Corp?”
2. Copilot Studio: Identifies the intent, uses the BC connector to query the Item table (Inventory) and the Sales Price table (customer-specific pricing).
3. Response: “We have 45 units in the Central Warehouse. The special price for Adatum is €150. Would you like me to create a draft quote?”
4. Extra Action: You can create a Sales Quote in BC.

**Impact:** Zero friction in sales, immediate response to the client.


## Prerequisites
- Microsoft account with appropriate licenses
- Access to Copilot Studio (https://copilotstudio.microsoft.com)
- Admin or maker permissions in your environment
- Agent from Lab_01

## Step 1: Access Copilot Studio

1. Navigate to [Microsoft Copilot Studio](https://copilotstudio.microsoft.com)
2. Click **Sign in** in the top right corner
3. Enter your Microsoft account credentials:
   - **Email/Username**: RedCarpetxx@CRMbc877736.onmicrosoft.com  (xx is a number between 01 and 60 assigned to you)
   - **Password**: the assigned password
4. Complete multi-factor authentication (MFA) if prompted


## Step 2: Open your previous Agent

1. Once logged in, click **Business Central Consulting XX** in the left navigation panel

## Step 3: Configure Agent Instructions

### Define Agent Instructions
1. Navigate to the **Instructions** section in the agent configuration
2. Add clear, specific instructions for your agent:
```
If you need to retrieve information from Business Central, use the MCP Business Central Server tool
```

## Step 4: Configure the MCP Server in Business Central

1. Open **Business Central** and seach for **MCP Server Configurations**


[Business Central](https://businesscentral.dynamics.com/b7e83739-3b6d-4d6a-8e7e-15c3afb4ce70/CPH)

   
   <img width="1023" height="252" alt="image" src="https://github.com/user-attachments/assets/b6e42d21-1e7b-430b-92d8-4858200057e8" />

3. Click **New**
4. As the name suggests **bcAgents**
5. Set **Dynamic Tool Mode**
6. Set **Discover additional Objects**
7. Set **Active**

   <img width="1259" height="601" alt="image" src="https://github.com/user-attachments/assets/97736479-d9c2-4bc7-91fa-41e83c420c47" />


## Step 5: Configure the tool in Copilot Studio

1. Click **Tools** in the menu
2. Click **Add a tool**
3. Search for **Model Context Protocol** and add it
   <img width="638" height="389" alt="image" src="https://github.com/user-attachments/assets/e5f0aaac-d0f5-46cc-ace4-ca79a86822c9" />

4. Create a connection
5. Click **Add and configure**
   <img width="1257" height="744" alt="image" src="https://github.com/user-attachments/assets/e08048a0-c174-49af-b4b5-72c800572fbc" />

6. Go to the **Inputs** area and introduce:
      - Environment: CPH
      - Company: CRONUS
      - MCP Server Configuration: bcAgents (same name as in **Business Central**)
        
   <img width="1099" height="532" alt="image" src="https://github.com/user-attachments/assets/f19f9d1c-0185-4052-a4ea-737f80d82bfe" />


## Step 6: Press the Save Button

## Step 7: Refresh the tools

   Press the refresh button to obtain the tools published for the MCP Server:

   <img width="1050" height="489" alt="image" src="https://github.com/user-attachments/assets/9336f47a-8488-4a5d-a393-90274791218c" />

## Step 8: Test Your Agent

1. Click the **Test** button in the top right corner
2. The test pane will open on the right side
3. Start a conversation to validate
4. Test with these prompts:

```
If you need to retrieve information from Business Central, use the MCP Business Central Server tool
```



## Best Practices for Agent Instructions

- **Be specific**: Clear instructions produce better results
- **Use examples**: Show the agent what good responses look like
- **Set boundaries**: Define what the agent should NOT do
- **Iterate**: Test and refine instructions based on real interactions
- **Document changes**: Keep track of instruction updates over time


---

**Last Updated**: December 2025  
**Version**: 1.1 -  Roberto Corella
