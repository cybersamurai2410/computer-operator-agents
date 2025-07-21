# Computer Operator using Parallel Multi-Agent AI
Implemented multi-agent AI system using LLMs to autonomously control a web browser within a virtual machine. Enabled agents to interpret goals, plan actions and execute sequences in a remote desktop by simulating human interaction. 

## Technical Architecture

The system is composed of:

* **Agent Core**: Coordinates multiple LLM-driven agents for planning and decision-making.
* **Browser Automation**: Executes actions (clicks, typing, navigation) within a virtual machine.
* **Streaming Interface**: Streams live updates of agent actions and task progress.
* **Configuration Layer**: Supports customization of environment and execution parameters.

## How It Works

1. **Initialization**: Load required environment variables and instantiate the agent graph.
2. **Task Definition**: User submits tasks via natural language prompts.
3. **Planning Phase**: Agents consult the LLM to generate a step-by-step action plan.
4. **Execution Phase**: The action plan is carried out in the virtual environment.
5. **Feedback Loop**: Results, logs, and screenshots are streamed back for monitoring.

## Customization Options

* **environment**: Select target platform (`ubuntu`, `windows`, or `web`).
* **prompt**: Define the system prompt to set context and objectives.
* **recursion\_limit**: Set the maximum number of agent iterations.
* **zdr\_enabled**: Enable or disable zero data retention for each request.

