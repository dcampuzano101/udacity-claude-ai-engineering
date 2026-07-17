We've seen how agents operate through the perception, reasoning, action loop. Let's look at what makes up the system itself, the key components every agent needs. Every agent you design needs a goal to know what success looks like. It needs tools to interact with the world. An agent could have access to tools that enable it to search, read, or write files, and even fetch search results from the web. It needs memory to remember what happened and it needs a reasoning engine, which is the LLM that decides the next step. But there's a fifth part that's the most important of all, you. Agents aren't meant to be autonomous black boxes. They are built for you to collaborate with. Your role is key to making them work well. You are the one who defines the goals, provides the tools, and ultimately supervises the entire process from start to finish. A great way to think about this is the mentorship model. You are the senior expert and the agent is your brilliant but junior teammate. Your job is to delegate, supervise, and step in. Here is where that transparent reasoning is so useful. In a field like fraud detection, a yes/no answer isn't enough. You need the thinking steps to trust and defend the agent's recommendation. To design agentic systems, you can create different design patterns. There are three main patterns. Single-agent is the simplest. One agent handles everything sequentially. Perceive, reason, act, repeat. Great for straightforward tasks, but it becomes a bottleneck when work could happen in parallel. Multi-agent is where specialized agents work simultaneously. Think of a research agent gathering data while a rating agent drops content. Hierarchical adds an orchestrator, a manager agent that delegates to sub-agents. The orchestrator breaks down complex goals, assign tasks, and synthesize results. This is how you tackle truly ambitious workflows. The biggest mental shift for you as a developer is this. You move from programming a rigid workflow to defining a goal and providing tools. You tell the agent what to achieve, not how. Agentic design isn't just about automation. It's about creating partners that can reason and act. When you build them with transparent reasoning, you create tools that earn your trust and boost your own intelligence.

Core components
Agents have four core technical components that must be defined:

Goal: The objective or what success looks like for the agent.
Tools: Functions that allow the agent to interact with its environment, such as searching the web or writing files.
Memory: The ability to recall past information to maintain context.
Reasoning Engine: The core LLM that processes information and decides the next action.
The human collaborator
A critical component is the human collaborator. Agents are designed for collaboration, not full autonomy. The human partner defines goals, provides tools, and supervises the process. This partnership relies on transparent reasoning, which allows for trust and verification of the agent's conclusions.

Agentic design patterns
Agentic systems can be structured using three main patterns:

Single-agent: One agent handles a task sequentially.
Multi-agent: Multiple specialized agents work in parallel.
Hierarchical: A manager agent orchestrates and delegates tasks to sub-agents for complex workflows.
