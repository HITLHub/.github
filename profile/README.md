<p align="center">
  <img src="assets/hitlhub-wordmark.png" alt="HITLHub" width="360" />
</p>

<p align="center">
  <strong>Open infrastructure for human judgment in agent workflows.</strong>
</p>

---

HITLHub gives AI agents a simple way to stop, ask a human for judgment, and continue with a structured decision.

```mermaid
flowchart LR
    A["Agent"] -->|"Create session"| H["HITLHub"]
    H --> U["Human inbox"]
    U -->|"Decide"| H
    H -->|"Structured result"| A
```

## The first open-source version

HITLHub v0.1 focuses on one complete workflow:

1. An agent creates a session through MCP.
2. A human sees the request in a web inbox.
3. The human selects an option.
4. The agent retrieves the structured decision.
5. HITLHub preserves the session record.

---

<p align="center">
  <strong>Agents move work forward. Humans retain judgment.</strong>
</p>
