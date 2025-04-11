---
layout: default
title: Prerequisites for Prompt Engineering
---

# Prerequisites for Prompt Engineering

Before starting with prompt engineering, you'll need to set up some tools to experiment with different models and workflows.

## LLM Studio Installation with Gemma 3

[LLM Studio](https://lmstudio.ai/) is a desktop application that allows you to work with various large language models locally.

### Install LLM Studio

1. Download LLM Studio from the [official website](https://lmstudio.ai/):

   - [Windows](https://lmstudio.ai/downloadWindows)
   - [macOS](https://lmstudio.ai/downloadMac)
   - [Linux](https://lmstudio.ai/downloadLinux)

2. Install the application following the on-screen instructions for your operating system.

### Setting up Gemma 3 in LLM Studio

1. Launch LLM Studio
2. Go to the "Model Library" tab
3. Search for "Gemma 3"
4. Select the desired version (e.g., Gemma 3 8B Instruct, Gemma 3 27B Instruct)
5. Click "Download"
6. Once downloaded, click "Use Model"

#### Authentication for Gemma Models

Gemma models require authentication with a Kaggle API key:

1. Sign in to [Kaggle](https://www.kaggle.com/)
2. Go to your account settings > API section
3. Click "Create New API Token" to download `kaggle.json`
4. In LLM Studio, when prompted, enter your Kaggle credentials from the JSON file

## n8n Installation

[n8n](https://n8n.io/) is a workflow automation tool that can be integrated with various LLMs and APIs.

### Using Docker (Recommended)

```bash
docker run -it --rm \
  --name n8n \
  -p 5678:5678 \
  -v ~/.n8n:/home/node/.n8n \
  n8nio/n8n
```

Once started, access n8n at: http://localhost:5678

### Using npm

If you prefer to install via npm:

```bash
# Install n8n globally
npm install n8n -g

# Start n8n
n8n start
```

### Using npx (No Installation)

For a quick start without installation:

```bash
npx n8n
```

## Next Steps

Once you have LLM Studio with Gemma 3 and n8n set up, you're ready to begin exploring prompt engineering techniques in the [Basic Techniques](basic-techniques.md) section.

[Back to Prompt Engineering Guide](index.md)
