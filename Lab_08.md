# Create a Pie Chart with the customers and Balances

## Prerequisites

- Access to Microsoft Copilot Studio
- Microsoft Dynamics 365 Business Central environment
- Business Central connector permissions



## Step 1: Access Your Agent in Copilot Studio

1. Navigate to [Microsoft Copilot Studio](https://copilotstudio.microsoft.com)
2. Sign in with your credentials
3. Create a new agent
4. Create two tools with **Find records**:  List of Items and List of Customers

   
   <img width="726" height="470" alt="image" src="https://github.com/user-attachments/assets/2117f364-eb44-4232-963e-eb7a932ae5ee" />


   
## Step 2: Activate the new functionality Code Interpreter

1. Click **Settings**
2. Select **Generative AI**
3. Go to **File Processing Capabilities** and activate **Code interpreter**

<img width="1641" height="420" alt="image" src="https://github.com/user-attachments/assets/e02e5f49-e44b-4701-8056-30804b93da25" />

## Step 3: Test Your Topic

1. Click **Save** in the top right
2. Click **Test** to open the test pane
3. Try these prompts:
```
  - Could you give me the list of customers with the balance?
  - Could you create a pie chart with the balance?  

  
```
<img width="522" height="480" alt="image" src="https://github.com/user-attachments/assets/070b47e7-0768-4c4d-a7e2-cd815a057bfd" />

4. Try these prompts:
```
  - Could you create a PDF document with the list and the chart?

```
<img width="811" height="656" alt="image" src="https://github.com/user-attachments/assets/848b37f9-f875-4740-9719-bc72e3c6fd1f" />

5. Try these prompts:
```
   pull a list of customers from Business Central. Then create a dashboard in Excel with analysis of customers, sales, balance, sales person.... Apply professional formating.
```

<img width="1826" height="753" alt="image" src="https://github.com/user-attachments/assets/8c518171-ad9a-413f-96ed-170229287c0a" />


## Resources

- [Business Central API Documentation](https://learn.microsoft.com/dynamics365/business-central/dev-itpro/api-reference/v2.0/)
- [Power Automate Connectors](https://learn.microsoft.com/connectors/dynamicssmbsaas/)
- [Copilot Studio Topics Guide](https://learn.microsoft.com/microsoft-copilot-studio/authoring-create-edit-topics)

---

**Congratulations!** You've successfully created a topic that reads customer data from Business Central and displays it conversationally in your Copilot agent.
