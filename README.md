# Udacity AI Engineering with Claude

A comprehensive repository for Udacity's AI Engineering course, featuring hands-on exercises, architectural designs, and video transcripts exploring multi-agent systems and agentic architecture patterns using Claude AI.

## 📚 Course Structure

### Lessons

- **lesson-01**: Model Selection & Classification
- **lesson-02**: Prompt Engineering & Optimization
- **lesson-03**: Agentic Architecture (Multi-Agent Design)
  - Exercise: Customer Support Ticket Routing System
  - 6 specialized agents with parallel execution
  - Complete architectural diagrams and analysis

*(Additional lessons to be added)*

### Video Transcripts

- **Agentic-System-Design/**
  - Components of Agentic Systems
  - Perception-Reasoning-Action Loop
  - Module Summary

- **Design-Agent-Architectures/**
  - Introduction to Agent Architectures
  - Demo Transcript & Implementation

## 🎯 Current Focus

### Lesson 03: Agentic Architecture - Customer Support Ticket Routing

A multi-agent system design for intelligent customer support ticket handling, processing 5,000+ tickets/day with <1hr enterprise SLA.

#### Architecture Components

**6 Specialized Agents:**
- **Triage Agent** (Sonnet) - Entry point, CRM lookup, categorization
- **Technical Agent** (Sonnet) - Code analysis, error logs, root cause
- **Billing Agent** (Haiku) - Account issues, payments, credits
- **Knowledge Base Agent** (Haiku) - Solution matching, FAQ lookup
- **Routing Agent** (Sonnet) - Decision logic, SLA rules
- **SLA Escalation Agent** (Haiku) - Background monitoring every 5 minutes

#### Key Diagrams

- `diagrams/multi-agent.mmd` → Multi-agent architecture with parallel execution
- `diagrams/workflow.mmd` → Complete ticket journey and decision flows
- `diagrams/sequence.mmd` → Interaction timeline with parallel agents
- `diagrams/sla-monitoring.mmd` → Escalation agent background monitoring

#### Performance Metrics

| Metric | Single-Agent | Multi-Agent |
|--------|-------------|------------|
| Processing Time | 30-60s | 8-12s |
| Daily Capacity | ~2,500 | 5,000+ |
| Auto-Resolution | ~20% | ~40% |
| SLA Compliance | ~70% | 92-95% |

## 📁 Repository Structure

```
.
├── README.md
├── .gitignore
├── cd14715-claude-code-classroom/     # Main course materials
│   ├── lesson-01/                     # Model selection
│   ├── lesson-02/                     # Prompt engineering
│   ├── lesson-03/                     # Agentic architecture
│   │   ├── demo/                      # Reference implementations
│   │   └── exercise/
│   │       └── starter/
│   │           ├── ARCHITECTURE.md    # Complete design doc
│   │           └── diagrams/          # Mermaid diagrams
│   └── ...
└── video-transcripts/                 # Course video notes
    ├── Agentic-System-Design/
    └── Design-Agent-Architectures/
```

## 🚀 Quick Start

### View Architecture Documentation

```bash
# Open the lesson-03 architecture document
cd cd14715-claude-code-classroom/lesson-03-agentic-architecture/exercise/starter
cat ARCHITECTURE.md

# View rendered diagrams (SVG format)
open diagrams/multi-agent.svg
open diagrams/workflow.svg
open diagrams/sequence.svg
open diagrams/sla-monitoring.svg
```

### Render Mermaid Diagrams

If you have `mmdc` installed:

```bash
mmdc -i diagrams/multi-agent.mmd -o diagrams/multi-agent.svg
mmdc -i diagrams/workflow.mmd -o diagrams/workflow.svg
mmdc -i diagrams/sequence.mmd -o diagrams/sequence.svg
mmdc -i diagrams/sla-monitoring.mmd -o diagrams/sla-monitoring.svg
```

Or use [Mermaid Live Editor](https://mermaid.live) to visualize `.mmd` files online.

## 📖 Key Learnings

### 1. Parallelization Wins for High-Volume Systems
- Sequential processing creates bottlenecks
- Parallel agents reduce 30-60s → 8-12s processing time
- Required for 5,000+/day volume with <1hr SLA

### 2. Agent Specialization Improves Quality & Cost
- Haiku (lightweight) for simple tasks: billing, FAQ matching
- Sonnet (capable) for complex reasoning: code analysis, routing
- Reduces costs by ~40% while maintaining quality

### 3. Background Agents Provide SLA Visibility
- Separate escalation agent monitors deadlines every 5 minutes
- Proactive alerting vs reactive firefighting
- Know which tickets are at risk BEFORE deadline

### 4. Failure Modes Cascade in Multi-Agent Systems
- One agent timeout affects all others
- Plan degraded modes: timeouts, fallbacks, circuit breakers
- Test failure scenarios as seriously as happy paths

## 🛠️ Technologies Used

- **Claude AI** (Sonnet, Haiku) - Multi-agent orchestration
- **Mermaid** - Architecture diagrams and flowcharts
- **Git** - Version control
- **TypeScript** - Exercise implementations (where applicable)

## 📝 Exercise Structure

Each lesson includes:
- **README.md** - Exercise overview and instructions
- **starter/** - Template code to complete
- **solution/** - Reference implementation
- **ARCHITECTURE.md** - Design documentation (when applicable)

## 🔄 Workflow for Syncing Between Computers

**Before starting work:**
```bash
git pull origin main
```

**After completing work:**
```bash
git add .
git commit -m "lesson-XX: description of changes"
git push origin main
```

## 📚 References

- [Claude API Documentation](https://claude.ai/docs)
- [Mermaid Diagram Syntax](https://mermaid.js.org)
- [Udacity AI Engineering Program](https://www.udacity.com)

## 📄 License

Course materials from Udacity. Personal exercises and notes.

---

**Last Updated:** July 17, 2026  
**Current Focus:** Lesson 03 - Agentic Architecture (Completed)  
**Next:** Lesson 04 - Specialized Agent Patterns
