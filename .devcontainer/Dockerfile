FROM node:24.6.0-trixie-slim

RUN apt update && \
    apt install -y \
    curl \
    git \
    locales \
    sudo \
    vim

# sudo
RUN echo "node ALL=(ALL) NOPASSWD:ALL" > /etc/sudoers.d/node && \
    chmod 0440 /etc/sudoers.d/node

# LOCALE
RUN sed -i 's/^# *\(en_US.UTF-8\)/\1/' /etc/locale.gen && \
    sed -i 's/^# *\(ja_JP.UTF-8\)/\1/' /etc/locale.gen && \
    locale-gen

# Node
RUN npm install -g \
    @anthropic-ai/claude-code \
    @google/gemini-cli \
    prettier
