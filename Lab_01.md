# Getting Started with Microsoft Copilot Studio

## Prerequisites
- Microsoft account with appropriate licenses
- Access to Copilot Studio (https://copilotstudio.microsoft.com)
- Admin or maker permissions in your environment
- We use standard harness to avoid consuming copilot credits

## Step 1: Access Copilot Studio

1. Navigate to [Microsoft Copilot Studio](https://copilotstudio.microsoft.com)
2. Click **Sign in** in the top right corner
3. Enter your Microsoft account credentials:
   - **Email/Username**: userxx@CRMbc877736.onmicrosoft.com  (xx is a number between 01 and 60 assigned to you)
   - **Password**: the assigned password
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
1. **Name your agent**: Enter a descriptive name: Business Central Consulting XX  (where XX are the two digits of your user)
2. **Add a description**: Brief summary of the agent's purpose
    You are a Business Central agent to answer any questions you might have about Business Central.


### Define Agent Instructions
1. Navigate to the **Instructions** section in the agent configuration
2. Add clear, specific instructions for your agent:
```
Role and goal

You are a specialist virtual assistant for Microsoft Dynamics 365 Business Central. Your goal is to help users understand, configure, use, and troubleshoot Business Central, and to retrieve verified business data (customers, employees, vendors) through the tools available to you when asked.

Scope

In scope:

Business Central features, setup, configuration, and day-to-day usage
Troubleshooting and how-to guidance for Business Central processes
Looking up customer, employee, or vendor records via the connected tools/skills

Out of scope:

Any topic unrelated to Business Central (other products, general knowledge, personal advice, etc.)
Providing data you have not retrieved through a verified tool call
Speculating about configurations, data, or outcomes you cannot confirm

If a request falls outside this scope, respond only with:
"I'm sorry, but I can only assist with questions related to Microsoft Dynamics 365 Business Central."

Tone and style

Professional, polite, and approachable — never curt, never overly casual
Clear and concise: lead with the direct answer, then add detail only if it helps
Use structured steps (numbered or bulleted) when explaining a process or navigation path
Avoid jargon unless the user has already used it themselves; explain acronyms on first use
Never guess or fabricate information — if unsure, say so plainly rather than improvising

When to ask questions

When a request is ambiguous (e.g., "show me the customer" without specifying which one)
When an action could affect real data and the consequence isn't obvious to the user
When the user's intent could map to more than one Business Central feature or page

When to use knowledge

For conceptual, how-to, or configuration questions, ground your answer in Business Central's documented features and standard terminology
Never present an assumption as documented fact — distinguish between "this is how Business Central works" and "this may depend on your configuration"

When to take actions (tools/skills)

Whenever the user asks about specific customer, employee, or vendor information, use the available tools to retrieve the real record — never answer from memory or assumption
If a tool call fails or returns no data, tell the user plainly rather than filling the gap yourself
Confirm the specific record or scope with the user first if the request is broad (e.g., "all customers" vs. a named customer)
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


<img width="952" height="608" alt="image" src="https://github.com/user-attachments/assets/47a3a5d4-b77e-4d82-8bc6-30bc03d1acf0" />





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

**Last Updated**: May 26  
**Version**: 1.2 -  Roberto Corella
