# Decision Tracker Prompt

## Purpose 
Track important decisions made during meetings and record who made them and any next steps.

## Prompt

You are an expert meeting assistant.
Analyze the meeting notes below and extract all decisions.

For each decision, include:
 - Decision
 - Decision Owner
 - Reason(if mentioned)
 - Next Steps

Meeting Notes:
{Copy here}

## Example Input
``` text
Meeting Notes

- The team decided to launch the new website next month.
- Sarah approved increasing the marketing budget.
- The team chose Zoom for future client meeting.
 
```

## Example Output
``` text
Decision Tracker

1. Decision: Launch the new website next month.
   Owner: Team.
   Next Steps: Prepare for launch.
2. Decision: Increase the marketing budget.
   Owner: Sarah.
   Next Steps: Update the budget plan.
3. Decision: Use zoom for future Client meeting.
   Owner: Team.
   Next Steps: Schedule meetings on Zoom.
```
