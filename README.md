<div style="background-color: #1e1e1e; color: #ffffff; padding: 30px; border-radius: 12px; font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;">
  
  <div style="text-align: center; margin-bottom: 30px;">
    <a href="https://gitee.com/yuanpluss">
      <img src="./background/image/新logo.png" alt="y-tian-plugin" style="width: 150px; height: 150px; border-radius: 50%;"/>
    </a>
  </div>

  <div style="display: flex; justify-content: center; gap: 15px; margin-bottom: 30px;">
    <a href="https://gitee.com/wan13877501248/y-tian-plugin">
      <img src="https://gitee.com/wan13877501248/y-tian-plugin/badge/star.svg?theme=dark" alt="Star" height="25">
    </a>
    <a href="https://gitee.com/wan13877501248/y-tian-plugin">
      <img src="https://gitee.com/wan13877501248/y-tian-plugin/badge/fork.svg?theme=dark" alt="Fork" height="25">
    </a>
    <img src="https://img.shields.io/badge/-JavaScript-eed718?style=flat-square&logo=javascript&logoColor=ffffff" alt="JavaScript" height="25">
    <img src="https://img.shields.io/badge/-Node.js-3C873A?style=flat-square&logo=Node.js&logoColor=white" alt="Node.js" height="25">
    <img src="https://img.shields.io/badge/Yunzai-V3.0.0-red?style=flat-square&logo=dependabot" alt="Miao-Yunzai" height="25">
    <a href="https://www.murphysec.com/console/report/1718228587458985984/1718228588025217024" style="display: block; width: 100%;">
    <img src="https://www.murphysec.com/platform3/v31/badge/1718228588025217024.svg" alt="Security Status" style="width: 100%; height: auto; max-width: 300px;">
   </a>
  </div>

  <h1 style="text-align: center; font-family: 'Courier New', monospace; letter-spacing: 2px;">😃 Cloudy Plugin Index Page</h1>

  <p style="text-align: center; font-size: 18px; font-family: 'Courier New', monospace;">
    Free online use
      <a href="https://yuanpluss.online:1111/" style="color: #00ffff;">AI</a>
    </strong>
  </p>

</div>

## ☁️ Plugin Introduction

### 🌟 Beacon

🌅 At first, we held a bright light  
Want to light the way for others  
We firmly believe that AI dividends should not be monopolized  
Every dreamer should have the opportunity to touch this world-changing technology

### 🌱 History
- Invest time and effort
- Build a free service platform
- Witness the continuous influx of users
- Gain gratitude and profit

### 🎯 Plugin Purpose

> **Y-Tian-Plugin** is a **Yunzai-Bot V3** plugin package that integrates multiple functions. It improves the versatility of the robot by integrating multiple AI models and entertainment functions.  
> Committed to providing users with free AI models to support daily life and learning, providing additional versions, professional versions and domestic solutions, integrating more than 100 popular large models, and free use of 100+ large models (including GPT-4/4-all, etc.).  
> **Note:** Illegal use (such as pornography, violence, politics, etc.) will result in the user's IP being blocked, please understand!

> 📢 **Most of the Ai in this project are free for charity, don't be deceived! **
> 📢 **The comprehensive free plan provided by Yuntian is an additional plan! **

### 🧠 AI Model Support

- **ChatGPT**, **Anthropic**, **ChatGLM**, **Gemini**, **Stable Diffusion**, **Midjourney**, **Suno**, **Pika**, **Bing**, **Copilot**, **Cohere** and other mainstream AI models
- Supports **text generation**, **image drawing**, **speech synthesis**, **AI composition**, **file processing**, **file generation** and other functions

### 🎪 Multi-function integration

- **AI integration**, **entertainment**, **game**, **learning**, **film** and other functions
- Rich command help to facilitate users to call various functions

### 💎 Free and Premium Features

- Provide a variety of free AI models
- Advanced features for sponsored users to experience in advance

## 📦 Installation Tutorial

In the root directory of **Yunzai-Bot**, run the command line tool and enter the following command:

### 1. Clone the repository (choose one)

- **Use Gitee (plugin, latest)**
  ```shell
  git clone --depth=1 https://gitee.com/wan13877501248/y-tian-plugin.git ./plugins/y-tian-plugin/
  ```

- **Using Gitee (plugin + V2 toolbox, under testing)**
  ```shell
  git clone --branch V2 --single-branch https://gitee.com/wan13877501248/y-tian-plugin.git ./plugins/y-tian-plugin/
  ```

- **Use Github (plugin, latest)**
  ```shell
  git clone --depth=1 https://github.com/yuanplussfive/y-tian-plugin.git ./plugins/y-tian-plugin/
  ```

### 2. Install dependencies

- **Enter the plugin directory**
  ```shell
  cd plugins/y-tian-plugin
  ```

- **Install dependencies** (recommended to use `pnpm` or `cnpm` in domestic environment)
  ```shell
  pnpm install
  ```

### Can I call the plugin free API in other scenarios? --Yes

 API endpoints:

```
 https://yuanpluss.online:3000/api/v1/chat/completions
```

Request parameters need to be passed through the request body in `JSON` format. The main parameters are as follows:

- `model`: The model ID to use, e.g. `gpt-4`.
- `messages`: An array containing the conversation messages. Each message is an object containing `role` and `content` properties.
- `temperature`: The sampling temperature, between 0 and 2, the higher the value, the more random the generated content.
- `top_p`: Alternative method for temperature sampling, only considering tokens that make up the top `top_p` probability mass.
- `n`: The number of completions to generate for each input message.
- `stream`: whether to return results incrementally.
- `stop`: After at most 4 sequences, the API will stop generating further markers.
- `max_tokens`: Maximum number of tokens to generate.
- `presence_penalty`: Penalize new tokens based on whether they have appeared in the text so far.
- `frequency_penalty`: Penalize new tokens based on how often they currently exist in the text.
- `logit_bias`: Modify the likelihood of a given token appearing in completions.
- `user`: A unique identifier representing the end user.

#### Example code

The following is a sample code for sending a request using JavaScript: (Obtained for free after key authorization)

```javascript
var myHeaders = new Headers();
myHeaders.append("Accept", "application/json");
myHeaders.append("Authorization", "Bearer {{YOUR_API_KEY}}");
myHeaders.append("User-Agent", "Apifox/1.0.0 (https://apifox.com)");
myHeaders.append("Content-Type", "application/json");

var raw = JSON.stringify([
   {
      "role": "user",
      "text": "Hello"
   }
]);

var requestOptions = {
   method: 'POST',
   headers: myHeaders,
   body: raw,
   redirect: 'follow'
};

fetch("https://yuanpluss.online:3000/api/v1/chat/completions", requestOptions)
   .then(response => response.text())
   .then(result => console.log(result))
   .catch(error => console.log('error', error));
```

<details>
  <summary>🤖 Postman debugging</summary>
  <img src="./background/image/Postman.png" alt="调试" width="100%">
</details>

## 🚀 Features at a glance

<details>
  <summary>🔍 Cloudy day help</summary>
  <img src="./background/image/Cloudy Help.jpg" alt="Cloudy Help" width="35%">
</details>



<details>
  <summary>🔍 Common help</summary>
  <img src="./background/image/Cloudy Help.jpg" alt="Cloudy Help" width="35%">
  <img src="./background/image/god Help.jpg" alt="god Help" width="39%">
  <img src="./background/image/chat Help.jpg" alt="chat Help" width="35%">
  <img src="./background/image/Additional Help.jpg" alt="Additional Help" width="48%">
</details>

## 🤖 AI Model Functionality Overview

### 💬 Conversation Model

#### 🌐 **OpenAI**

| Model Name | Functional Description |
|----------|------|
| gpt-3.5-turbo | Basic dialogue model |
| gpt-4o-mini | Lightweight version of GPT4, optimized response speed |
| gpt-4 | Advanced dialogue model, supporting more complex tasks |
| gpt-4-32k | Extended context length, suitable for long document processing |
| gpt-4-vision | Conversational model supporting image input |
| gpt-4-dalle | A model that combines GPT4 and DALL-E to understand and generate creative images. |
| gpt-4-all | Multifunctional GPT4 model, integrating multiple processing capabilities: **Networking**, **Image Recognition**, **Drawing**, **File Analysis**, **Code Interpreter** |
| gpt-4o-all | Multifunctional version of GPT4 model, integrating multiple processing capabilities: **Networking**, **Image Recognition**, **Drawing**, **File Analysis**, **Code Interpreter** |
| gpt-4-gizmo | A variant of GPT4, focusing on specific application scenarios, can use all gpts plug-ins, and integrates multiple processing capabilities: **Networking**, **Image Recognition**, **Drawing**, **File Analysis**, **Code Interpreter** |
| o1-mini-all | Official plus version, with thought process display, o1-mini is a fast, cost-effective reasoning model designed for coding, mathematics and scientific use cases. The model has 128K context and the latest database. |
| o1-preview-all | Official plus version, with thought process shown, o1-preview is OpenAI's new reasoning model for complex tasks, often used to handle complex tasks. The model has 128K context and the latest database. |
| ... | ... |

#### 🧠 **Anthropic**

| Model Name | Functional Description |
|----------|------|
| claude-3-haiku-20240307 | Lightweight version of the Claude model V3 series with the fastest response speed |
| claude-3-opus-20240229 | The latest version of the Claude model, featuring state-of-the-art language processing techniques |
| claude-3-5-sonnet-20240620 | The latest version of the Claude model, more powerful and cheaper than Opus, with the most advanced language processing technology |
| ... | ... |

#### 🔍 **Google**

| Model Name | Functional Description |
|----------|------|
| gemini-pro | Google's advanced AI model provides more sophisticated language understanding and generation capabilities |
| gemini-pro-vision | Google's advanced AI model for image recognition |
| gemini-1.5-pro | Google advanced AI model, complex reasoning tasks such as code and text generation, text editing, problem solving, data extraction and generation, support image recognition |
| gemini-1.5-flash | Google advanced artificial intelligence model, lightweight version, supports image recognition |
| ... | ... |

#### 🔍 **Bing**

| Model Name | Functional Description |
|----------|------|
| Bing-Creative | Bing Creative mode, good at divergence |
| Bing-Practice | Bing rigorous mode, rigorous thinking |
| Bing-Balanced | Bing-Balanced mode, balanced answers |
| ... | ... |

#### 🦾 **Meta**

| Model Name | Functional Description |
|----------|------|
| llama-2-7b | Lightweight Language Model |
| llama-3-sonar-large-32k-chat | Large chat model, supporting long context |
| code-llama-70b-instruct | Focus on code generation and understanding |
| ... | ... |

#### 🤖 **ChatGLM**

| Model Name | Functional Description |
|----------|------|
| glm-4 | Zhipu AI general large model provides more powerful question-answering and text generation capabilities. Suitable for complex dialogue interactions and deep content creation and design scenarios. |
| glm-4v | Zhipu AI general large model realizes the deep integration of visual language features and supports various image understanding tasks such as visual question answering, image captioning, visual positioning, and complex target detection. |
| glm-4-alltools | ChatGLM with multiple tools integrated |
| glm-4-plus | ChatGLM with enhanced capabilities |
| ... | ... |

#### 🌟 **Mixtral**

| Model Name | Functional Description |
|----------|------|
| mixtral-8x7b | Medium Mixtral Model |
| mistral-34b | Large Mixtral model, suitable for complex tasks |
| ... | ... |

#### ⚙️ **Other Models**

| Model Name | Functional Description |
|----------|------|
| webgpt | Suitable for web content processing and generation |
| mj-chat | Midjourney combined with gpt4 dialogue model |
| deepseek-chat | Chinese comprehensive ability (AlignBench) The strongest among open source models, and in the same echelon as closed source models such as GPT-4-Turbo and Wenxin 4.0 in the evaluation. Chat only |
| ... | ... |

### 🖼️ Wenshengtu Model

#### 🎨 **Stability**

- **Stable Diffusion Series**
  - High quality image generation
  - Multiple styles support

#### 🌈 **Flux**

- **Flux Series**
  - Fast image generation
  - Flexible style adjustment

#### 🎨 **playground**

- **playground-v2/3 series**
  - High quality image generation
  - Multiple styles support

#### 🖌️ **PixArt**

- **PixArt Series**
  - Artistic style image generation
  - Support multiple art genres

#### 🌌 **Midjourney**

- **Midjourney/Niji Series**
  - Highly detailed image generation
  - Multiple styles support

#### 🖍️ **OpenAI**

- **DALL-E Series**
  - Creative image generation
  - Support image generation

#### 🌈 **ideograms**

- **ideogram-V2 series**
  - Fast image generation
  - Good at art style

#### 🖼️ **Others**

- **Stable Cascade**, **dream...** 等

### 🔍 Image recognition model

#### 📝 **OCR**

- **Text Recognition**
  - High-precision text extraction
  - Multi-language support

#### 🌐 **OpenAI**

- **gpt-4-v/all series multimodal GPT models**
  - Support mixed input of images and text
  - Strong understanding and generation ability

#### 🤖 **ChatGLM**

- **glm-4-alltools series of multifunctional models**
  - Integrate multiple tools
  - Support image analysis

#### 🔍 **Google**

- **gemini-pro-vision series professional vision models**
  - Advanced image recognition
  - Professional application support

#### 🖼️ **Others**

- ...

### 🔊 Voice Model

#### 🎤 **Virtual Idol**

- **Genshin Impact Level 3 Voice**
- **Fish-vits Voice**

#### 🎵 **Song Generation**

- **Suno-V3**
- **Suno-V3.5**

#### 🗣️ **OpenAI**

- **tts/tts-1-hd...**

### 🎥 Video Model

#### 📹 **Runway**
#### 🎬 **Watch**
#### 📺 **Previous**

## 🤖 Commonly used basic settings

### 💎 Plan interval settings

<details>
  <summary>🔷 Open partitions (individual independent conversations)</summary>
  
  **Command example:**
  - `#xx open partition interval`
  - `#Switch xx preset xx`
</details>

<details>
  <summary>🔷 Close partitions (group chat shared conversation)</summary>
  
  **Command example:**
  - `#xxClose partition interval`
  - `#Switch xx preset xx`
</details>

### 💎 Image dialogue rendering method

#### 🔷 Use MathJax (good at rendering mathematical formulas, accurate)

<details>
  <summary>Example 1</summary>
  <img src="./background/image/math_1.jpg" alt="MathJax 示例1" width="400"/>
</details>

<details>
  <summary>Example 2</summary>
  <img src="./background/image/math_2.jpg" alt="MathJax 示例2" width="400"/>
</details>

#### 🔷 Use Markdown (good at rendering code blocks and highlighting)

<details>
  <summary>Example 1</summary>
  <img src="./background/image/markdown_1.jpg" alt="Markdown 示例1" width="400"/>
</details>

<details>
  <summary>Example 2</summary>
  <img src="./background/image/markdown_2.jpg" alt="Markdown 示例2" width="400"/>
</details>

### 💎 TTS voice reply

#### 🔷 Enable TTS first Reply

<details>
  <summary>Example</summary>
  <img src="./background/image/tts_1.png" alt="Turn on TTS reply" width="400"/>
</details>

#### 🔷 View TTS sound

<details>
  <summary>Example</summary>
  <img src="./background/image/tts_2.png" alt="View TTS sound" width="400"/>
</details>

#### 🔷 Select TTS tone

<details>
  <summary>Example</summary>
  <img src="./background/image/tts_3.png" alt="Select TTS tone" width="400"/>
</details>

## 🤖 AI function display

### 💎 Multimodal partial model function display

#### 📄 File handling and generation

<details>
  <summary>📄 File generation</summary>
  <img src="./background/image/all_1.jpg" alt="File generated" width="400"/>
</details>

<details>
  <summary>📄 File processing</summary>
  <img src="./background/image/all_3.jpg" alt="File processing" width="400"/>
</details>

#### 🎨 Plus DALL-E drawing

<details>
  <summary>🎨 DALL-E Vincent's Picture</summary>
  <img src="./background/image/all_2.jpg" alt="DALL-E Vincent Photo" width="400"/>
</details>

<details>
  <summary>🎨 DALL-E raw image</summary>
  <img src="./background/image/all_4.jpg" alt="DALL-E raw image" width="400"/>
</details>

#### 🔍 Deep web search

<details>
  <summary>🔍 Information Retrieval</summary>
  <img src="./background/image/all_5.jpg" alt="Information Retrieval" width="400"/>
</details>

<details>
  <summary>🔍 Retrieval generation</summary>
  <img src="./background/image/all_6.jpg" alt="Search and generate" width="400"/>
</details>

#### 🖼️ Image retrieval and recognition

<details>
  <summary>🖼️ Image retrieval</summary>
  <img src="./background/image/all_7.jpg" alt="Image retrieval" width="400"/>
</details>

<details>
  <summary>🖼️ Image analysis</summary>
  <img src="./background/image/all_8.jpg" alt="Image Analysis" width="400"/>
</details>

### 💎 Function display of some domestic models

#### 🌙 Dark Side of the Moon Web Version

<details>
  <summary>🌙 Click to view</summary>
  <img src="./background/image/kimi.jpg" alt="Dark Side of the Moon Web Version" width="400"/>
</details>

#### 🌟 Spark Model Web Version

<details>
  <summary>🌟 Click to view</summary>
  <img src="./background/image/星火.png" alt="星火Model Web Version" width="400"/>
</details>

#### 🧠 Zhipu Qingyan Web version

<details>
  <summary>🧠 Click to view</summary>
  <img src="./background/image/glm4.png" alt="Zhipu Qingyan Web Version" width="400"/>
</details>

#### 🐉 Baichuan Intelligent Web Version

<details>
  <summary>🐉 Click to view</summary>
  <img src="./background/image/百川.png" alt="百川智能网页版" width="400"/>
  <img src="./background/image/百川2.png" alt="百川智能网页版2" width="400"/>
</details>

#### 🖥️ Microsoft Copilot

<details>
  <summary>🖥️ Click to view</summary>
  <img src="./background/image/copilot_1.jpg" alt="微软 Copilot 1" width="400"/>
  <img src="./background/image/copilot_2.jpg" alt="微软 Copilot 2" width="400"/>
  <img src="./background/image/copilot_3.jpg" alt="微软 Copilot 3" width="400"/>
</details>

#### 🤖 Tongyi Qianwen Web Version

<details>
  <summary>🤖 Click to view</summary>
  <img src="./background/image/qwen_1.jpg" alt="Tongyi Qianwen Web Version 1" width="400"/>
  <img src="./background/image/qwen_2.jpg" alt="Tongyi Qianwen Web Version 2" width="400"/>
</details>

#### 🔍 DeepSeek Web Edition

<details>
  <summary>🔍 Click to view</summary>
  <img src="./background/image/deepseek.png" alt="DeepSeek Web版" width="400"/>
</details>

## 🔆 Interaction process with AI

### 💻 Dialogue Interaction

> Cloudy Help → AI General Help → Open At Reply → Select Enabled Plan → Reference Plan Help (Additional models can be used for free after authorization by Xiaobai, and this plan is recommended)

<details>
  <summary>📈 Click to view the flowchart</summary>
  <img src="./background/image/zs.jpg" alt="Interaction flow chart" width="400"/>
</details>

## Feedback and Support

If you have any comments or suggestions about this plugin, please feel free to give us feedback through the following channels:

### 💬 Let's talk together

**[Click to join the Y-Tian plugin exchange group (authorized free additional models)](http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=jZAmTxqiEMP_hDTQOH4yaU-VgIuezmAQ&authKey=C3gEwvelMi3MKAdU87muZmN11eg3ewtIRvbjupFAZtEZoPwKRa6Rii1fmKD85iUw&noverify=0&group_code=912701273)**

Here you can communicate with developers and other users, ask questions, share experiences, and more.

### ⭐ Star support

If you like our plugin, please give ⭐️ Star in the relevant repository, which will be our motivation to move forward!

### 💰 Sponsorship channels

You can also support us through the following channels:

- [Afdian](https://afdian.com/a/yuan_20)  
  Sponsored users will have the opportunity to experience unannounced new features of this plugin in advance. Your support will be our motivation for continuous updates!

### ✨ Contributing members

![Contributors](https://img.shields.io/badge/all_contributors-3-orange.svg?style=flat-square)

<a href="https://github.com/yuanplussfive/y-tian-plugin/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=yuanplussfive/y-tian-plugin" />
</a>

![Alt](https://repobeats.axiom.co/api/embed/b0e531137448010a6b4b2e307afbd67e39c00d49.svg "Repobeats analytics image")

### 🚪 Portal

The following are related links to resources for this project:

- ☁️ **Cloudy plugin Yunzai-Bot version**
  - [Github](https://github.com/yuanplussfive/y-tian-plugin)
  - [Gitee](https://gitee.com/wan1387501248/y-tian-plugin)
- ☁️ **Cloudy plugin Alemon-Bot version**
  - [Gitee](https://gitee.com/wan13877501248/y-tian-plugin-for-alemon-bot)
- 😺 **Meow version Yunzai-Bot (V3)**
  - [Github](https://github.com/yoimiya-kokomi/Miao-Yunzai)
  - [Gitee](https://gitee.com/yoimiya-kokomi/Miao-Yunzai)
- 💻 **Same demo web AI dialogue**
  - [Demo1](https://gitee.com/yuanpluss/simple-free-ai)
  - [Demo2](https://gitee.com/yuanpluss/demo-chatai)
- 💻 **One-click deployment for personal Windows computers**
  - [Gitee](https://gitee.com/wan13877501248/yin-tian-tian-script-for-win)

### 🙏 Acknowledgements

We would like to express our sincere gratitude to all the individuals and organizations who have contributed to this project, as well as the sponsoring members of Aidianfa! If you have any questions or feedback, please contact us via the following methods:

- 📧 Email: [email@yuanoop.com](mailto:email@yuanoop.com)
- 💬 Exchange group: **[Plugin Exchange Group](http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=jZAmTxqiEMP_hDTQOH4yaU-VgIuezmAQ&authKey=C3gEwvelMi3MKAdU87muZmN11eg3ewtIRvbjupFAZtEZoPwKRa6Rii1fmKD85iUw&noverify=0&group_code=912701273)**

> 📢 **It is strictly forbidden to use this project for any commercial purpose and illegal behavior! **
