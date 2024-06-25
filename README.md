# Building Agentic RAG with LlamaIndex

## Key Aspects

### Router Agent

- A router agent is the simplest form of an agent in the RAG framework. It functions by selecting one of several predefined query engines to execute a query. For instance, it can choose between a Q&A engine and a summarization engine based on the type of query it receives.

- **Objective:** Build an agent that can route queries to the appropriate engine, thereby providing relevant responses.

- **Implementation:** You will use a decision-making process where the agent evaluates the query and decides whether it is best handled by the Q&A engine or the summarization engine.

### Tool Calling

- This involves adding more advanced functionality to the router agent by enabling it to call external tools and infer arguments to pass to these tools.

- **Objective:** Enhance the router agent so that it can not only select a function to execute but also determine the appropriate parameters or arguments for that function.

- **Implementation:** The agent will utilize an LLM (Large Language Model) to understand the query context and infer necessary arguments for the tool it selects. This might involve understanding the nuances of the query to decide the best way to handle it.

### Research Assistant Agent

- The research assistant agent is an advanced agent capable of multi-step reasoning. Unlike the router agent, which makes a single decision, the research assistant can engage in a more complex decision-making process involving multiple steps and tools.

- **Objective:** Build an agent that can conduct a series of operations over time, using multiple tools and steps to arrive at a comprehensive answer.

- **Implementation:** This involves creating a loop where the agent iterates over tools and queries, adjusting its approach based on intermediate results. For example, it might start by summarizing a document and then use the summary to perform a detailed Q&A session.

### Multi-Document Handling

- In this section, you'll extend the research assistant agent to handle queries that involve multiple documents. This is crucial for complex tasks where information needs to be gathered and synthesized from various sources.

- **Objective:** Enable the agent to perform comprehensive research by accessing and integrating information from multiple documents.

- **Implementation:** The agent will be designed to manage and compare information from several documents, potentially summarizing and cross-referencing data to provide a well-rounded response.

### Additional Learning Aspects

- **Debugging and Control:** Techniques to debug the agents you build, ensuring they perform as expected. This includes strategies for monitoring the agents' actions and outcomes.
