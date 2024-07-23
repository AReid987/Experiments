FROM python:3.12-slim

# Install git and other dependencies
RUN apt-get update && apt-get install -y git && rm -rf /var/lib/apt/lists/*

# Install aider
RUN pip install --no-cache-dir aider-chat
RUN pip install --no-cache-dir aider-chat[browser]

# Set up a non-root user
RUN useradd -m aider
USER aider

# Set working directory
WORKDIR /workspace

# Set environment variables
ENV PYTHONUNBUFFERED=1
ENV TERM=xterm-256color
ENV GROQ_API_KEY=${GROQ_API_KEY}
ENV AIDER_GUI=${AIDER_GUI}
ENV AIDER_DARK_MODE=${AIDER_DARK_MODE}

# Run aider with tty allocation
ENTRYPOINT ["aider", "--model", "groq/llama3-70b-8192"]
