<img width="928" height="940" alt="image" src="https://github.com/user-attachments/assets/afeef3fa-e282-40c5-9707-52389ab38fe3" />


# PromptChain Tutorial

PromptChain is a single-page HTML tool for chaining multiple prompts together when working with Ollama models. This README is a quick tutorial for getting the app running locally in your browser.

## 1. Download the HTML file
Download `PromptChainV6.html` (or clone this repository) and keep the file somewhere on your computer.

## 2. Open it in your browser
Double-click the HTML file or drag it into your browser. Because the entire interface lives in one HTML document, there is no build step or server to start.

## 3. Make sure Ollama is installed
PromptChain relies on your local Ollama installation for inference, so install Ollama if you have not already. Once installed, keep the Ollama service running in the background while you use PromptChain. The app works completely offline because every call is routed to your local Ollama runtime—no cloud APIs involved.
https://ollama.com/download/windows

## 4. Configure CORS for browser access
Ollama enforces CORS restrictions by default. Set the `OLLAMA_ORIGINS=*` environment variable (or a more restrictive value that includes `file://`) before starting Ollama so that your browser can reach the local API from the standalone HTML file.

On Windows, do this:

Open Control Panel → System → Advanced system settings

Click Environment Variables…

Under User variables (or System variables if you want it global), click New…

Variable name: OLLAMA_ORIGINS

Variable value (for development): *

Later you can tighten it to http://localhost:8000 if you want.

Click OK until all dialogs are closed.

## 5. Chain prompts
With the page open and Ollama running, start creating prompt chains to explore different reasoning steps or personas. Each prompt in the chain feeds into the next, allowing you to craft richer multi-step interactions.

That's it—download, open in your browser, ensure Ollama is installed with the proper CORS configuration, and you're ready to chain prompts offline.
