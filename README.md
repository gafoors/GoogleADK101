# GoogleADK101

# CodeLabs from Google
- [GoogleADK101](#googleadk101)
- [CodeLabs from Google](#codelabs-from-google)
  - [ADK Crash Course - From Beginner To Expert](#adk-crash-course---from-beginner-to-expert)
      - [Summary](#summary)
    - [ADK Web](#adk-web)
  - [Evaluating Agents with ADK](#evaluating-agents-with-adk)
    - [Youtube Videos](#youtube-videos)
    - [In Pictures](#in-pictures)


## ADK Crash Course - From Beginner To Expert
https://codelabs.developers.google.com/onramp/instructions#0

1. Learning Roadmap 
   ![Learning Roadmap](./resources/agents/ADKLearningRoadmap.png)
2. Loop Agent 
   ![Loop Agent](./resources/agents/IterativePlanningLoopAgent.png)


#### Summary
You've completed the Enhanced ADK Adventure! You have successfully. Let's review the advanced orchestration patterns you've successfully implemented:

**The Router Pattern**: You built a master router agent capable of analyzing user intent and delegating tasks to the appropriate specialist agent or workflow.

**Sequential Workflows**: Using SequentialAgent, you elegantly chained agents together, creating clean, readable code for multi-step tasks without manual data handling.

**Iterative Refinement**: You constructed a sophisticated feedback loop with LoopAgent, enabling your agents to plan, self-critique, and improve their output until it met specific constraints.

**Parallel Power**: You maximized speed and efficiency by using ParallelAgent to run multiple research tasks concurrently, later synthesizing the results into a unified response.


### ADK Web

1. Clone the Repository
   Open Terminal and run:
   ```
    git clone https://github.com/cuppibla/ADK_Basic.git
    cd ADK_Basic
    ```
2. Set Up Virtual Environment and Install Dependencies
   * Option A: Automated Setup (Recommended)
    Run the setup script
    ```
    chmod +x setup_venv.sh
    ./setup_venv.sh
    ```
    * Option B: Manual Setup
    1. Create virtual environment
   
        `uv venv -p 3.13 .adk_env`

    2. Activate virtual environment
        `source .adk_env/bin/activate`

    3. Install dependencies
        ```
        pip install --upgrade pip
        pip install -r requirements.txt
        ```
3. 🔥 IMPORTANT - Create Environment Variables

    ⚠️ Don't skip this step! 
    
    Create a .env file in the working directory:

    * Create the .env file

        `touch .env`

    * Add these lines to the file:

        ```
        GOOGLE_GENAI_USE_VERTEXAI=FALSE
        GOOGLE_API_KEY=your_actual_api_key_here
        ```
        🚨 CRITICAL: Replace your_actual_api_key_here with your actual API key!

4. Activate Virtual Environment (if not already active)

    `source .adk_env/bin/activate`

    You should see (.adk_env) at the beginning of your terminal prompt.

5. Run the ADK Web Interface

    `adk web`

6. Open Your Browser
    
    Open your browser and go to the URL shown in terminal (usually http://localhost:8000)
    In the top-left dropdown, select agent
    Start chatting with your day trip planning agent!

## Evaluating Agents with ADK
https://codelabs.developers.google.com/adk-eval/instructions#0

### Youtube Videos
1. [Agent Evaluation - Intro](https://www.youtube.com/watch?v=WZZLtwnZ4w0)
2. [Evaluate Agents in Practice](https://www.youtube.com/watch?v=vuBvf7ZRKTA&list=TLPQMDQwMTIwMjahuEXWq4Dvmg&index=2)

### In Pictures
![Agent System Components](./resources/eval/AgentSytemComponents.png)
![Agent System Testing](./resources/eval/AgentSystemLevelTesting.png)
![Agent Testing Pyramid](resources/eval/AgentTestingPyramid.png)
![Summary](resources/eval/AgentEvaluation.png)

