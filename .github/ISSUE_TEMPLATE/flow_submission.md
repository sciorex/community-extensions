---
name: Flow Submission
about: Submit a new flow to the community repository
title: '[FLOW] '
labels: new-flow
assignees: ''
---

## Flow Information

**ID**: <!-- lowercase-hyphenated, e.g., my-flow -->
**Name**: <!-- Display name -->
**Version**: <!-- e.g., 1.0.0 -->

## Description

<!-- Clear description of what your flow does -->

## Use Cases

<!-- List specific use cases this flow addresses -->
1.
2.
3.

## Technical Details

### Required Agents

<!-- List agents this flow depends on -->
- [ ] Uses community agents (list them):
- [ ] Uses custom agents (included in PR):

### Trigger Type

<!-- How is this flow triggered? -->
- [ ] Manual
- [ ] Schedule (cron)
- [ ] Ticket Created
- [ ] Ticket Updated

### Node Structure

<!-- Brief description of the flow's node structure -->

```
Trigger → [Node 1] → [Node 2] → End
                  ↘ [Condition] → ...
```

## Testing

<!-- How did you test this flow? -->

- [ ] Tested locally in Sciorex
- [ ] Ran full execution
- [ ] Tested all branches/conditions
- [ ] Tested error handling

## Checklist

- [ ] I have read the [CONTRIBUTING.md](../CONTRIBUTING.md)
- [ ] I have read and agree to the [CLA](../CLA.md)
- [ ] My flow follows the naming conventions
- [ ] All required agents are available or included
- [ ] I have updated `index.json` with my flow metadata
- [ ] `requiredAgents` field is correctly populated

## Additional Notes

<!-- Any other information about your flow -->
