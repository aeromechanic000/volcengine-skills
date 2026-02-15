---
name: volc-image-skill
description: Generate and edit high-quality images using Volcengine Doubao models.
---

# Image Generation Instructions
When the user asks for an image:
1. Use the `volc-img` MCP tools to generate the request.
2. Ask for specific dimensions (e.g., 1024x1024) if not provided.
3. Always save the resulting image to a local path (e.g., `./outputs/image.png`) and confirm the filename to the user.
