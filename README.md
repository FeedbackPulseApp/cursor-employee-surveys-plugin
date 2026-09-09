# Employee Surveys by FeedbackPulse

Cursor Marketplace plugin for FeedbackPulse’s remote MCP server. Design a company-specific employee survey through a short guided conversation, review the full design before signing in, then optionally connect FeedbackPulse to save the exact approved version as a reusable template or an unlaunched draft.

Survey design is currently supported in **English**.

## Install

Once listed on the [Cursor Marketplace](https://cursor.com/marketplace), install from **Customize → Marketplace** (or the plugin page). Cursor will connect the remote MCP and prompt for OAuth when you save a design.

Manual / custom connect (same production endpoint):

```json
{
  "mcpServers": {
    "employee-surveys-feedbackpulse": {
      "url": "https://app.feedbackpulse.com/mcp/employee-surveys"
    }
  }
}
```

MCP URL: `https://app.feedbackpulse.com/mcp/employee-surveys`  
Transport: remote Streamable HTTP with OAuth/PKCE

## What this does

- Design employee surveys before you create a FeedbackPulse account
- Refine a complete proposal in chat
- Optionally OAuth-connect to save the **exact** approved design as a reusable template or an **unlaunched** draft

## What this does not do

- eNPS analytics, benchmarks, or score reporting
- Survey launch, scheduling, reminders, or respondent management
- Results or engagement dashboards

eNPS may appear only as an **optional survey question** when it fits the decision you are designing for.

The only authenticated write is persistence of an approved design (`survey-design:persist`). Anonymous design tools work before sign-in.

## Starter prompts

1. Design a five-minute engagement survey for a company facing retention risk.
2. Create a culture-change survey, then help me refine anything that misses the mark.
3. Design a survey, then help me choose a reusable template or an unlaunched draft.
4. Help me design a short survey about leadership trust for a 120-person company.

## Links

- Product: https://feedbackpulse.com/
- Privacy: https://feedbackpulse.com/privacy-policy
- Terms: https://feedbackpulse.com/terms-of-service
- Support: https://feedbackpulse.com/support

## Note on Cursor channels

This repository is for the **official** [Cursor Marketplace](https://cursor.com/marketplace/publish). The community directory at [cursor.directory](https://cursor.directory) is a separate listing path.

## License

MIT
