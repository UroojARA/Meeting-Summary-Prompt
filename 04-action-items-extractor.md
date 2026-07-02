# Action Items Extractor Prompt

## Purpose
Extract action items, owners, deadlines, priorities, and blockers from meeting notes.

## Prompt
Your are an expert project coordinator.

Analyze the meeting notes below and extract all action items.

For each action item, include
  - Task
  - Owner
  - Deadline
  - Priority
  - Status

Use this table format:
|#|Task|Owner|Deadline|Priority|Status|
|-|----|-----|--------|--------|------|

Also include:
## Unassigned Tasks
## Upcoming Deadlines
## Risks or Blocker

Meeting notes:
{copy here}

## Example Input

```text
Payment Meeting Notes

- John will send the overdue payment reminder to ABC Ltd by Friday.
- Maria will prepare the payment report by Monday.
- The refund for Client A is awaiting approval.
```

## Example Output

|#|Task|Owner|Deadline|Priority|Status|
|-|----|-----|--------|--------|------|
|1|Send overdue payment reminder to ABC Ltd|John|Friday|High|Pending|
|2|Prepare payment report|Maria|Monday|Medium|Pending|
|3|Obtain approval for Client A refund|Not Assigned|Not Mentioned|Medium|Pending|

### Unassigned Tasks
 - Obtain approval for Client A refund

### Upcoming Deadlines
 - John: Send payment reminder by Friday.
 - Maria: Prepare payment report by Monday.

### Risks or Blocker
 - Client A refund cannot be processed until approval is received.
