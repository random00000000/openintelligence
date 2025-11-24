<img width="1059" height="874" alt="image" src="https://github.com/user-attachments/assets/aba7daf4-7b32-4cc6-96cc-4c1153b2fecf" />


1. Download the HTML file
Download OllamaMultiAgent v7.html (or clone this repository) and keep the file somewhere on your computer.

2. Open it in your browser
Double-click the HTML file or drag it into your browser. Because the entire interface lives in one HTML document, there is no build step or server to start.

3. Make sure Ollama is installed
PromptChain relies on your local Ollama installation for inference, so install Ollama if you have not already. Once installed, keep the Ollama service running in the background while you use OllamaMultiAgent v7. The app works completely offline because every call is routed to your local Ollama runtime—no cloud APIs involved. https://ollama.com/download/windows

4. Configure CORS for browser access
Ollama enforces CORS restrictions by default. Set the OLLAMA_ORIGINS=* environment variable (or a more restrictive value that includes file://) before starting Ollama so that your browser can reach the local API from the standalone HTML file.

On Windows, do this:

Open Control Panel → System → Advanced system settings

Click Environment Variables…

Under User variables (or System variables if you want it global), click New…

Variable name: OLLAMA_ORIGINS

Variable value (for development): *

Later you can tighten it to http://localhost:8000 if you want.

Click OK until all dialogs are closed.
