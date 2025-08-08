# Agent Development Kit

Agent Development Kit (ADK) is a flexible and modular framework for developing and deploying AI agents. While optimized for Gemini and the Google ecosystem, ADK is model-agnostic, deployment-agnostic, and is built for compatibility with other frameworks. ADK was designed to make agent development feel more like software development, to make it easier for developers to create, deploy, and orchestrate agentic architectures that range from simple tasks to complex workflows.

## ✨ Key Features
Rich Tool Ecosystem: Utilize pre-built tools, custom functions, OpenAPI specs, or integrate existing tools to give agents diverse capabilities, all for tight integration with the Google ecosystem.

Code-First Development: Define agent logic, tools, and orchestration directly in Python for ultimate flexibility, testability, and versioning.

Modular Multi-Agent Systems: Design scalable applications by composing multiple specialized agents into flexible hierarchies.

Deploy Anywhere: Easily containerize and deploy agents on Cloud Run or scale seamlessly with Vertex AI Agent Engine.

## Quickstart

1. Copy `.env.example` to `.env`, and set up your config:

```shell
GOOGLE_GENAI_USE_VERTEXAI=FALSE
GOOGLE_API_KEY=PASTE_YOUR_ACTUAL_API_KEY_HERE
```

2. Install the dependencies:

```shell
pip install -r requirements.txt
```

3. Run the code:
```shell
adk web
```

Example output:

```shell

22:41:00 with symbolk in awesome-agent-quickstart/google-adk on  main [!?] using ☁️  default/veo-test-461409 via 🅒 agent took 1m 36.4s 
➜ adk web
INFO:     Started server process [37497]
INFO:     Waiting for application startup.

+-----------------------------------------------------------------------------+
| ADK Web Server started                                                      |
|                                                                             |
| For local testing, access at http://localhost:8000.                         |
+-----------------------------------------------------------------------------+

INFO:     Application startup complete.
INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
```

4. Open the browser and go to `http://localhost:8080` to see the development UI, select agent and talk to it:
```shell
What's the time and weather in New York?
```


# References

- [ADK Doc](https://google.github.io/adk-docs/)
- [GitHub Repository](https://github.com/google/adk-python)