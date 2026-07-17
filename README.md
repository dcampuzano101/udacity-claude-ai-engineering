# Udacity AI Engineering with Claude

Personal working repository for the Udacity "AI Engineering with Claude" course. Synced between personal and work computers via git.

## Status Legend

| Symbol | Meaning |
|--------|---------|
| ✅ | Complete or ready to run |
| 🚧 | In Progress |
| ⬜ | Not Started |

## Course Progress

| # | Lesson | Topic | Status | Path |
|---|--------|-------|--------|------|
| 0️⃣ | **warm-up** | Getting Started with Your Workspace | ✅ | [`lesson-00-warm-up`](cd14715-claude-code-classroom/lesson-00-warm-up) |
| 1️⃣ | **model-selection** | Support Ticket Classifier (Haiku/Sonnet/Opus Routing) | ✅ | [`lesson-01-model-selection`](cd14715-claude-code-classroom/lesson-01-model-selection) |
| 2️⃣ | **extended-thinking** | Extended Thinking for Fraud Detection | ⬜ | [`lesson-02-extended-thinking`](cd14715-claude-code-classroom/lesson-02-extended-thinking) |
| 3️⃣ | **agentic-architecture** | Multi-Agent Customer Support System | ✅ | [`lesson-03-agentic-architecture`](cd14715-claude-code-classroom/lesson-03-agentic-architecture) |
| 4️⃣ | **claude-code-config** | Configure Claude Code for Support Ticket System | ⬜ | [`lesson-04-claude-code-config`](cd14715-claude-code-classroom/lesson-04-claude-code-config) |
| 5️⃣ | **agent-sdk** | Contract Standardizer | ⬜ | [`lesson-05-agent-sdk`](cd14715-claude-code-classroom/lesson-05-agent-sdk) |
| 6️⃣ | **custom-tools** | API Validator | ⬜ | [`lesson-06-custom-tools`](cd14715-claude-code-classroom/lesson-06-custom-tools) |
| 7️⃣ | **structured-outputs** | Meeting Notes Analyzer | ⬜ | [`lesson-07-structured-outputs`](cd14715-claude-code-classroom/lesson-07-structured-outputs) |
| 8️⃣ | **claude-skills** | JavaScript Code Reviewer | ⬜ | [`lesson-08-claude-skills`](cd14715-claude-code-classroom/lesson-08-claude-skills) |
| 9️⃣ | **mcp-integration** | Code Quality Reviewer | ⬜ | [`lesson-09-mcp-integration`](cd14715-claude-code-classroom/lesson-09-mcp-integration) |
| 🔟 | **multi-agent-orchestration** | Sales Opportunity Qualifier | ⬜ | [`lesson-10-multi-agent-orchestration`](cd14715-claude-code-classroom/lesson-10-multi-agent-orchestration) |
| 1️⃣1️⃣ | **tdd-with-ai** | TDD Strategy for a Shopping Cart Module | ⬜ | [`lesson-11-tdd-with-ai`](cd14715-claude-code-classroom/lesson-11-tdd-with-ai) |
| 1️⃣2️⃣ | **evaluating-agents** | Tip Calculator / Sentiment Analysis Evaluators | ⬜ | [`lesson-12-evaluating-agents`](cd14715-claude-code-classroom/lesson-12-evaluating-agents) |
| 1️⃣3️⃣ | **computer-use** | Form Automation Agent | ⬜ | [`lesson-13-computer-use`](cd14715-claude-code-classroom/lesson-13-computer-use) |
| 📦 | **project** | Enterprise Multi-Agent Code Review Orchestrator | ⬜ | [`project`](cd14715-claude-code-classroom/project) |

## Completed Lessons

### Lesson 03 — Agentic Architecture ✅

**Multi-Agent Customer Support Ticket Routing System** — A comprehensive architecture design for intelligent ticket handling at scale (5,000+ tickets/day, <1hr enterprise SLA).

→ **Full details** in [`lesson-03-agentic-architecture/exercise/starter/ARCHITECTURE.md`](cd14715-claude-code-classroom/lesson-03-agentic-architecture/exercise/starter/ARCHITECTURE.md)

**Quick snapshot:**
- 6 specialized agents (Triage, Technical, Billing, Knowledge Base, Routing, SLA Escalation)
- Parallel execution: 8–12s processing vs 30–60s sequential
- 4 fully rendered Mermaid diagrams (multi-agent flow, workflow, sequence, escalation logic)
- Failure mode analysis with mitigations

---

## Video Transcripts

Course video notes for reference:

### Agentic System Design
- [`components-agentic-system.md`](video-transcripts/Agentic-System-Design/components-agentic-system.md) — Core components of agentic systems
- [`perception-reasoning-action-loop.md`](video-transcripts/Agentic-System-Design/perception-reasoning-action-loop.md) — The PRA loop explained
- [`module-summary.md`](video-transcripts/Agentic-System-Design/module-summary.md) — Module recap

### Design Agent Architectures
- [`intro.md`](video-transcripts/Design-Agent-Architectures/intro.md) — Introduction to architecture patterns
- [`demo-transcript.md`](video-transcripts/Design-Agent-Architectures/demo-transcript.md) — Sales agent demo (single vs multi-agent)

---

## Repository Structure

```
.
├── README.md (this file)
├── .gitignore
├── cd14715-claude-code-classroom/          ← All course lessons
│   ├── lesson-00-warm-up/
│   ├── lesson-01-model-selection/
│   ├── lesson-02-extended-thinking/
│   ├── lesson-03-agentic-architecture/     (✅ COMPLETE)
│   │   ├── demo/
│   │   └── exercise/starter/
│   │       ├── ARCHITECTURE.md             (full design doc)
│   │       └── diagrams/                   (Mermaid + SVG)
│   ├── lesson-04 … lesson-13/
│   └── project/                            (capstone)
└── video-transcripts/
    ├── Agentic-System-Design/
    └── Design-Agent-Architectures/
```

Each lesson typically contains:
- `demo/` — Reference implementation
- `exercise/starter/` — Template to complete
- `exercise/solution/` — Full solution for reference

---

## Workflow: Syncing Between Computers

### Before Starting Work

Always pull latest changes:

```bash
cd ~/Documents/current_projects/udacity-ai-engineering-with-Claude
git pull origin main
```

### After Completing Work

Commit and push your changes:

```bash
git add .
git commit -m "lesson-XX: description of changes"
git push origin main
```

### Example Flow

**Personal computer:**
```bash
git pull                                  # Get any work from the other computer
# ... work on lesson-05 ...
git add .
git commit -m "lesson-05: complete agent-sdk contract standardizer exercise"
git push origin main
```

**Work computer (next day):**
```bash
git pull                                  # Gets the lesson-05 work from personal computer
# ... continue with lesson-06 or other tasks ...
```

---

## Quick Links

- 📖 [Udacity AI Engineering Program](https://www.udacity.com)
- 🤖 [Claude API Docs](https://claude.ai/docs)
- 📊 [Mermaid Diagram Syntax](https://mermaid.js.org)
- 🔧 [Claude Code CLI](https://github.com/anthropics/claude-code)

---

**Repository:** https://github.com/dcampuzano101/udacity-claude-ai-engineering  
**Last Updated:** July 17, 2026
