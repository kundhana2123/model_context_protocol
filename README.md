# model_context_protocol
* It tells how LLM applications get access to the tools and data resources. 
* In coversation between the mcp client hosted inside your own LLM application and an MCP server that will expose tools and data resources, prompts to the LLM aplication. 
* MCP will provide tools, prompt templates and resources to the chatbot.
* MCCP standardizes how AI applications interact with external systems. 
* Many different AI applications are talking to a similar data source but written in a different way. 

* MCP is based on a client-server architecture. The client's job is to find tools and resources. The server's job is to expose that information to the client.

* MCP transports: This will handle the underlying mechanics of how meesages are sent and received. 
server runned locally -> stdio
servers runned remotely -> 1. http + sse(stateful connection)
                            2. streamable http (allows stateful or stateless connection)
