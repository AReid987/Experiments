<!-- SECTION - Heading -->
# A Turborepo of Experiments

-----------------------------------------------------------------------
<!-- SECTION - Title -->
## **Learning and Experimenting with Technology**

<!-- ANCHOR - Experiment Category -->
### Software Engineering Agents

#### Query: Can two AI agents collaborate on code?

Testing OpenDevin and Aider and how they might collaborate

#### Environment

    - Turborepo Monorepo
    - Docker Compose
    - Docker containers
            - OpenDevin
            - Aider
            - Tailscale for networking
            - TBD
    - Tailscale
        - Intra cluster communication
        - Remote access
        - VPN, VPC, VPS

#### Goals

##### Build and Deploy a simple web app with modern tech

- Stack
  - Frontend
    - Next.js
    - TailwindCSS
  - Backend
    - TBD
  - Database
    - TBD
  - CI/CD / DevOps
    - GitHub Actions
    - Husky
    - Conventional Commits
    - CommitLint
    - Commitizen

##### Evaluate Ability for Agentic Collaboration

     - Can Aider and OpenDevin haromoniously plan, design and execute a functional web app?
     - Will they have awareness of each other in the sense that they are influenced?
     - Can they ingest the other into context?
     - Will they have awareness of the environment?

##### Phase One Preparation

Starting from blank code base

- **Human interaction**
- Containerize Agents
- Start containers
- Enable networking between container
- Mount volumes to containers for Agent access to filesystem

- **Agentic Birth**
- Establish Plan
- Initialize turborepo
- Initalize git
- begin building

<!-- ----------------------------------------------------------------------- -->
<!-- TODO - Find the rest of my AI Agents and tools and categorize them -->

<!-- ### Agents

Local

IDE

TERMINAL

IDE EXTENSION

STANDALONE

- ?? Composer ??
- Cursor
- AIChat - [github](https://github.com/sigoden/aichat)
- Aider - [docs](https://aider.chat/docs/install/install.html)
- Fabric - [github](https://github.com/danielmiessler/fabric)
- Groq AI Tools - [github](https://github.com/RMNCLDYO/groq-ai-toolkit)
- Open Devin - [github](https://github.com/OpenDevin/OpenDevin?tab=readme-ov-file#-getting-started)
- Warp
- Cody
- Continue
- Blackbox
- Claude
- TabNine
- Codeium
- Amazson Q
- Gitub Copilot
- LMStudio
- AnythingLLM
- Jan
- Drawthings
- Ollama
- Wave
- AppMap
- Codiumate
- Frontier
- Jupyter
- Mintlify
- Sourcery
- Tabby
- Traycer -->