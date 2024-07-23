<!-- SECTION - Heading -->

# A Turborepo of Experiments

---

<!-- SECTION - Title -->

## **Currently Testing**

<!-- ANCHOR - Experiment Category -->

### Software Engineering Agents

#### Query: Can AI Software Engineer Agents collaborate to create function code?

Testing OpenDevin and Aider and how they might collaborate

#### Environment

    - Turborepo Monorepo
    - Docker Compose
    - Docker containers
            - OpenDevin
            - Aider
            - Tailscale for networking
            - Nginx web server
    - Tailscale
        - Intra Node comms
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


##### **Human interaction**

- Init git repo
- Init Turborepo
- Containerize Agents
- Start containers
- Enable networking between container
- Mount volumes to containers for Agent access to filesystem

- **Agentic Birth**

  - Establish Plan
  - begin building

##### Project Structure

```
agentic-rubrics/
┣ .anima/
┃ ┣ cache/
┃ ┗ .gitignore
┣ .turbo/
┃ ┣ cache/
┃ ┣ cookies/
┃ ┗ daemon/
┣ .vscode/
┃ ┣ diff/
┃ ┗ settings.json
┣ AgenticPlanning/
┃ ┗ harpa-transcripts.json
┣ apps/
┃ ┣ aider/
┃ ┣ docs/
┃ ┣ open-devin/
┃ ┣ tailscale/
┃ ┗ web/
┣ packages/
┃ ┣ eslint-config/
┃ ┣ shared-config/
┃ ┣ typescript-config/
┃ ┗ ui/
┣ shared_workspace/
┃ ┣ .aider.chat.history.md
┃ ┗ aider
┣ tailscale/
┃ ┣ files/
┃ ┣ derpmap.cached.json
┃ ┣ tailscaled.log.conf
┃ ┣ tailscaled.log1.txt
┃ ┣ tailscaled.log2.txt
┃ ┗ tailscaled.state
┣ .env
┣ .gitignore
┣ .npmrc
┣ Mindmap-1.html
┣ docker-compose.bak.yml
┣ docker-compose.yml
┣ nginx.conf
┣ package.json
┣ pnpm-lock.yaml
┣ pnpm-workspace.yaml
┣ tree.txt
┗ turbo.json
```


Notes

- created containers, docker compose yaml for services
- configuring tailscale
- used Harpa with Claude to extract from youtube video by tailscale

Summary:
Alex from Tailscale provides a quick-start guide for using Docker with Tailscale. He demonstrates how to install Docker on a fresh Ubuntu server, create a Tailscale container, and connect it to a Tailnet. The video covers deploying multiple applications (Nginx and Sterling PDF) using Docker Compose, securing them with Tailscale, and setting up HTTPS certificates using Tailscale Serve. Alex emphasizes the simplicity of connecting containers to a Tailnet and accessing them from anywhere, regardless of network topology.

Step-by-step instructions:

1. Install Docker:
   a. Run the get.docker.com script
   b. Execute: sudo sh install-docker.sh
   c. Add user to Docker group: usermod -aG docker `<username>`
   d. Log out and log back in
   e. Verify installation: docker run --rm hello-world
2. Create first Tailscale container:
   a. Create a Docker Compose YAML file
   b. Add Tailscale and Nginx services to the file
   c. Generate an auth key from Tailscale admin dashboard
   d. Add the auth key to the Docker Compose file
   e. Run: docker compose up -d
3. Deploy additional applications (e.g., Sterling PDF):
   a. Add Sterling PDF service to Docker Compose file
   b. Generate OAuth client credentials in Tailscale admin console
   c. Add OAuth client secret to Docker Compose file
   d. Set up necessary volumes and network configurations
   e. Run: docker compose up -d
4. Set up HTTPS certificates with Tailscale Serve:
   a. Enable HTTPS certificates in Tailscale admin console
   b. Create a JSON configuration file for Tailscale Serve
   c. Add TS_Serve_Config to Docker Compose file
   d. Restart containers: docker compose up -d
   e. Verify HTTPS setup using docker exec command
5. Access your containerized services:
   a. Use Tailscale DNS names or assigned hostnames
   b. Access services securely over HTTPS

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
