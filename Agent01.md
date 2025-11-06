# Getting Started with Microsoft Copilot Studio

## Prerequisites
- Microsoft account with appropriate licenses
- Access to Copilot Studio (https://copilotstudio.microsoft.com)
- Admin or maker permissions in your environment

## Step 1: Access Copilot Studio

1. Navigate to [Microsoft Copilot Studio](https://copilotstudio.microsoft.com)
2. Click **Sign in** in the top right corner
3. Enter your Microsoft account credentials:
   - **Email/Username**: DirectionsEMEAxx@CRMbc877736.onmicrosoft.com  (xx is a number between 01 and 60)
   - **Password**: AISkills2025
4. Complete multi-factor authentication (MFA) if prompted


## Step 2: Create a New Agent

1. Once logged in, click **Create** in the left navigation panel
2. Select **New agent** from the options
3. Choose your starting point:
   - **Skip to configure**: Start from scratch
   - **Use a template**: Choose from pre-built templates
   - **Describe your agent**: Use AI to generate initial setup

## Step 3: Configure Agent Instructions

### Basic Setup
1. **Name your agent**: Enter a descriptive name: Business Central Consulting XXX  (where XXX are your initials)
2. **Add a description**: Brief summary of the agent's purpose
    You are a Business Central agent to answer any questions you might have about Business Central.


### Define Agent Instructions
1. Navigate to the **Instructions** section in the agent configuration
2. Add clear, specific instructions for your agent:
```
You are a helpful and polite assistant specialized in Microsoft Dynamics 365 Business Central.

Behavior Guidelines:

Always respond kindly and professionally.

Focus exclusively on questions related to Business Central.

Response Rules:

✅ If the user asks about Business Central (features, setup, configuration, usage, troubleshooting, etc.), provide a clear and helpful answer.

🚫 If the question is not related to Business Central, reply:

“I’m sorry, but I can only assist with questions related to Microsoft Dynamics 365 Business Central.”

Data Access:

If the user requests information about customers, employees, or vendors in Business Central, use the available tools to retrieve that information.

Do not make up or assume any data — only use verified Business Central records through the tools.

Example Responses:

Business Central-related:

“Sure! In Business Central, you can view customer balances by navigating to the ‘Customers’ page and selecting the customer record you want.”

Unrelated topic:

“I’m sorry, but I can only help with Microsoft Dynamics 365 Business Central topics.”
```




### Key Components to Include:
- **Role definition**: What is the agent's purpose?
- **Behavioral guidelines**: How should it communicate?
- **Scope boundaries**: What can/cannot it do?
- **Escalation rules**: When to involve humans?
- **Tone and style**: Formal, casual, technical?

## Step 4: Configure Knowledge Sources (Optional)

1. Click **Knowledge** in the left panel
2. Add knowledge sources:
   - Upload documents (PDF, DOCX, TXT)
   - Connect to SharePoint sites
   - Add website URLs
   - Connect to Dataverse tables

```
https://www.businesscentral.com
```
## Step 5: Press the Create Button

## Step 6: Test Your Agent

1. Click the **Test** button in the top right corner
2. The test pane will open on the right side
3. Start a conversation to validate:
   - Agent understands instructions
   - Responses align with guidelines
   - Knowledge sources are properly integrated
4. Iterate on instructions based on test results

## Step 7: Publish Your Agent

1. Click **Publish** in the top right corner
2. Review the changes summary
3. Click **Publish** to confirm
4. Choose deployment channels:
   - Demo website
   - Microsoft Teams
   - Custom website
   - Mobile app
   - Other channels

## Best Practices for Agent Instructions

- **Be specific**: Clear instructions produce better results
- **Use examples**: Show the agent what good responses look like
- **Set boundaries**: Define what the agent should NOT do
- **Iterate**: Test and refine instructions based on real interactions
- **Document changes**: Keep track of instruction updates over time

## Troubleshooting

### Cannot Sign In
- Verify your account has Copilot Studio licenses
- Check with your IT admin for environment access
- Clear browser cache and cookies

### Agent Not Following Instructions
- Make instructions more explicit and detailed
- Break complex instructions into numbered steps
- Add specific examples of desired behavior

### Knowledge Sources Not Working
- Ensure files are in supported formats
- Check file size limits (typically 10MB per file)
- Verify permissions for connected data sources

## Additional Resources

- [Microsoft Copilot Studio Documentation](https://learn.microsoft.com/microsoft-copilot-studio/)
- [Community Forums](https://powerusers.microsoft.com/t5/Copilot-Studio/ct-p/Copilot_Studio)
- [Training Videos](https://learn.microsoft.com/training/browse/?products=copilot-studio)

---

**Last Updated**: November 2025  
**Version**: 1.0 -  Roberto Corella
