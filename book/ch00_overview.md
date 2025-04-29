# Building Multi-Agent Research Assistants with LangGraph

## [Preface](ch00_preface.md)
- About this book
- Who this book is for
- What you'll learn
- Prerequisites

## [Chapter 1: Introduction to LangGraph and Multi-Agent Systems](ch01.md)
- What is LangGraph?
- Understanding directed state flow graphs
- Multi-agent systems vs. single-agent workflows
- The research assistant use case
- Overview of the research assistant architecture

## [Chapter 2: System Architecture and Components](ch02.md)
- High-level architecture overview
- Understanding StateGraph and MessagesState
- Key components:
  - Schema definitions
  - Node functions
  - Edge management
  - State handling
- The role of Send() API for parallel processing

## [Chapter 3: Schema Design and Data Modeling](ch03.md)
- Core data modeling with Pydantic
- Building a state management system
- Understanding the type hierarchy:
  - GenerateAnalystsState
  - InterviewState
  - ResearchGraphState
- Designing composable states
- Annotated fields and operators

## [Chapter 4: Creating AI Analyst Personas](ch04.md)
- Defining the Analyst model
- Implementing the Perspectives model
- Using structured output with LLMs
- Setting up the persona generation process
- Handling human feedback in the workflow

## Chapter 5: Building the Interview System
- The interview state machine
- Question generation techniques
- Information retrieval strategies:
  - Web search implementation
  - Wikipedia retrieval
- Implementing expert answers
- Tracking conversation turns
- Router logic for conversation flow

## Chapter 6: Document Retrieval and Context Management
- Working with TavilySearchResults
- Implementing WikipediaLoader
- Formatting search documents
- Context accumulation with Annotated lists
- Citations and source management

## Chapter 7: Section Writing and Report Generation
- Technical writing prompts and strategies
- Structured section creation
- Introduction and conclusion generation
- Flow control for section assembly
- Source citation management

## Chapter 8: Graph Construction and Execution Flow
- Building the state graph
- Adding nodes and edges
- Implementing conditional routing
- Handling interruptions for human feedback
- Parallel execution with Send() API

## Chapter 9: Managing State Across Sub-Graphs
- Nested state graph architecture
- Passing state between parent and child graphs
- Reducing multiple outputs to a single state
- Managing completions and interruptions

## Chapter 10: Prompting Strategies for Research Assistants
- Designing effective system prompts
- Structured output for consistency
- Managing source citations
- Balancing exploration and focus
- Tone and style considerations

## Chapter 11: Error Handling and Robustness
- Handling unexpected LLM outputs
- Fallback strategies for search failures
- User feedback integration points
- Debugging state flow issues
- Graceful error recovery

## Chapter 12: Advanced Patterns and Extensions
- Adding more analyst types
- Extending the search capabilities
- Implementing additional sources
- Custom report formatting options
- Interactive feedback mechanisms

## Chapter 13: Deployment and Production Considerations
- Scaling multi-agent systems
- Managing API costs
- Handling long-running processes
- Monitoring and logging
- User experience design

## Appendix A: LangGraph Core Concepts
- State graphs in depth
- Message passing patterns
- Human-in-the-loop workflows
- Conditionals and branching

## Appendix B: Complete Code Reference
- Full annotated code listing
- Configuration options
- Extension points

## Appendix C: Prompt Engineering Guide
- System message design patterns
- Output formatting techniques
- Ensuring consistent responses
