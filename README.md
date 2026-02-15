# Volcengine Skills for Claude Code

A unified suite of skills and MCP servers for **Claude Code**, enabling high-performance image and video generation using Volcengine's Doubao (豆包) models directly from your terminal.

## 🚀 Features

- **Image Generation**: Create and edit high-fidelity images using `volcengine-image-mcp`.
- **Cinematic Video**: Generate 5-10 second cinematic clips from text or reference images using `volcengine-video-mcp` (Doubao-Seedance).
- **Local Workflow**: Automatically handles local file saving for generated assets.
- **Unified Setup**: Install both capabilities with a single command.

## 📦 Installation

To add this marketplace and install the plugin suite, run the following commands in Claude Code:

```bash
# 1. Add the marketplace
/plugin marketplace add aeromechanic000/volcengine-skills

# 2. Install the plugin suite
/plugin install aeromechanic@volcengine-skills

```

### 🔑 Authentication

You must have a Volcengine (Ark) API Key. It is recommended to set this in your environment variables:

```bash
export DOUBAO_API_KEY="your_api_key_here"

```

## 🛠 Usage

Once installed, Claude gains new "skills" that allow it to understand creative prompts.

### Image Generation

Simply ask Claude to create an image. It will use the `volc-img` MCP server.

> "Create a minimalist 3D render of a futuristic office in 1024x1024."

### Video Generation

Claude will use the `volc-vid` MCP server (defaulting to `doubao-seedance-1-5-pro-251215`).

> "Generate a 5-second cinematic video of a spaceship entering a nebula, slow camera zoom."

## 📂 Project Structure

* `.claude-plugin/`: Manifest files (`plugin.json`, `marketplace.json`) for Claude Code integration.
* `skills/image-gen/`: Instructions for image generation and editing.
* `skills/video-gen/`: Instructions for cinematic video prompting and image-to-video workflows.

## 🤝 Credits

This project bundles the following MCP servers:

* [volcengine-image-mcp](https://github.com/aeromechanic000/volcengine-image-mcp)
* [volcengine-video-mcp](https://github.com/aeromechanic000/volcengine-video-mcp)
