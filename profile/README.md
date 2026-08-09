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
3. The human selects an option and may add a justification.
4. The agent retrieves the structured decision.
5. HITLHub preserves the session record.

### MCP tools

```text
create_session
get_session
cancel_session
```

### Core capabilities

- 👤 Human decisions only
- 💬 Questions with structured options
- ⏳ Integration-defined expiration
- 🧾 Basic session and decision history
- 🐳 A fully containerized deployment
- 🐘 PostgreSQL as the source of truth

If time expires, HITLHub records that no human decision was made. It never invents or automates a response.

```bash
docker compose up
```

No Kafka, microservices, teams, notifications, attachments, or complex approval workflows in the first version—just the smallest useful human-in-the-loop system.

---

<p align="center">
  <strong>Agents move work forward. Humans retain judgment.</strong>
</p>
