<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->

<a name="readme-top"></a>

<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->

<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->

<!-- PROJECT LOGO -->
<div align="center">
    <img src="https://github.com/open-mindware/AutoGPT-Mindware/assets/23727727/6d982e1b-ffff-4fe5-9820-04441f8e77d2" alt="Logo" width="200" height="200">
</div>

## 📚 Prerequisites

### 1. Obtain OpenAI API Key

If you don't already have an OpenAI API key, get one [here](https://openai.com/blog/openai-api).

### 2. Obtain Mindware API Key

Sign up to [Mindware](https://mindware.xyz) and locate your free API key on the account page:

<img width="945" alt="Screenshot 2023-08-27 145759" src="https://github.com/open-mindware/AutoGPT-Mindware/assets/23727727/00583046-3468-4bfe-b32d-5a6c76009068">

### 3. Install Docker Desktop

If you don't already have Docker, download and install the latest version [here](https://www.docker.com/products/docker-desktop).

## 🔧 Setup

### 1. Install AutoGPT & Mindware

To install AutoGPT and the Mindware plugin, make sure Docker is running and execute the following command in a directory of your choosing:

#### For Mac, Linux, or WSL:

```bash
git clone https://github.com/open-mindware/AutoGPT-Mindware-Installer.git && cd ./AutoGPT-Mindware-Installer && ./installer.sh
```

#### For Windows (Powershell):

```powershell
git clone https://github.com/open-mindware/AutoGPT-Mindware-Installer.git; cd AutoGPT-Mindware-Installer; .\installer.bat
```

### 3. Run AutoGPT

Whenever you want to run AutoGPT after the installation process, run the following command from the AutoGPT directory:

```bash
docker compose run --rm auto-gpt --install-plugin-deps
```

## 🧠 How to Use

After completing the installation and configuration steps, you can enable specific plugins for AutoGPT via the [plugin portal](https://mindware.xyz). For instance, if you want AutoGPT to find YouTube videos, enable the YouTube plugin:

<img width="945" alt="Screenshot 2023-08-27 151437" src="https://github.com/open-mindware/AutoGPT-Mindware/assets/23727727/bcdb83bd-36e3-4993-b6ac-83660ef1cc0d">

### Example:

#### 1. Configure AutoGPT

Set up the `ai_settings.yaml` file with the following parameters:

```yaml
ai_goals:
  - Find YouTube videos on how to make Otoro nigiri.
ai_name: FoodTubeGPT
ai_role:
  An AI-powered virtual assistant that specializes in helping users find and
  obtain specific cooking videos on YouTube.
api_budget: 0.05
```

#### 2. Run AutoGPT

Launch AutoGPT. It should utilize the YouTube plugin to find sushi videos 🍣

