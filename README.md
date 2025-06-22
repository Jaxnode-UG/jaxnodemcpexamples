# JaxNode June 25th MCP example code

This is the sample code for the JaxNode June 2025 presentation on Model Context Protocol.

This example workspace has three projects in the `apps` folder. They are as follows:

* apps/avmxmcpstdio - This is a MCP server running a MCP server using STDIO
* apps/avmxmcpserver - This is MCP server running Express so it can do HTTP Streaming
* apps/avwxchat - This is a Next.js app using a LLM consuming the MCP Server

# Installing the examples

These examples require Node.js 22 or higher and PNPM since this is being run from a PNPM workspace.

To install, run the following command at the root level of the workspace folder:

```sh
$ pnpm install
```

This example uses OpenAI, but you can change this to use any LLM that supports tool calling through Langchain's React and MCP plugins. The default expects an OpenAI API Key. You can get one by going to [https://platform.openai.com/](https://platform.openai.com/), and going to your settings and selecting `API Keys`.

You can either add your API key to your environment variables, but you also rename the `.env.example` to `.env.local`, and setting the `OPENAI_API_KEY="<YOUR_API_KEY>"` to your API key.

To run the example, simply run `pnpm run dev` at the root of the project.

Copyright 2025 JaxNode
