**The Pain:** The finance team spends hours drafting invoice reminder emails and looking up which invoices are overdue.

**The Exercise:** An agent that drafts (or sends) emails based on the actual account status.

**Flow:**
1. The user asks the Agent: “Give me a summary of Trey Research’s outstanding balance and draft an email requesting payment for invoices over 30 days past due.”
2. Copilot Studio: Queries the Customer Ledger Entry table in BC, filters by Due Date, and sums amounts.
3. Uses Generative AI to write a formal but friendly email, inserting invoice numbers and exact amounts.
4. Output: Displays the draft in the chat or opens an Outlook window ready to send.

## Prerequisites
- Microsoft account with appropriate licenses
- Access to Copilot Studio (https://copilotstudio.microsoft.com)
- Admin or maker permissions in your environment

## Step 1: Access Copilot Studio

1. Navigate to [Microsoft Copilot Studio](https://copilotstudio.microsoft.com)
2. Click **Sign in** in the top right corner
3. Enter your Microsoft account credentials:
   - **Email/Username**: RedCarpetxx@CRMbc877736.onmicrosoft.com  (xx is a number between 01 and 60 assigned to you)
   - **Password**: the assigned password
4. Complete multi-factor authentication (MFA) if prompted

## Step 2: Use this prompt

```
Give me a summary of Trey Research’s outstanding balance and draft an email requesting payment for invoices over 30 days past due.

```

## Step 3 (optional if you have email): Send directly the email

1. Click **Tools**
2. Click **Add Tool**
3. Filter for **Model Context Protocol**

<img width="880" height="388" alt="image" src="https://github.com/user-attachments/assets/eb205151-acec-452b-8448-0866343f481e" />

4. Search for **Email Management MCP Server**
5. Create a connection
6. Review the tools added

   <img width="944" height="622" alt="image" src="https://github.com/user-attachments/assets/388ce567-3545-4db0-8977-4639b470c47f" />

## Step 4: Test the agent and modify the prompt to send the email

NOTE: Modify the customer's email to send you the information before using it.

```
Give me a summary of Trey Research’s outstanding balance and write an email requesting payment for invoices over 30 days past due.

```

<img width="497" height="281" alt="image" src="https://github.com/user-attachments/assets/24b0a211-819a-47f4-9c6e-48161346d388" />


## Step 5: The email will be sent to the customer

<img width="924" height="381" alt="image" src="https://github.com/user-attachments/assets/3cb8882a-f4cd-4b13-b0bc-4579d7391290" />

---

**Last Updated**: December 2025  
**Version**: 1.1 -  Roberto Corella
