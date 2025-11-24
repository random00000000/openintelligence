# MultiAgent Meeting (Standalone HTML)

![MultiAgent Meeting interface](https://github.com/user-attachments/assets/aba7daf4-7b32-4cc6-96cc-4c1153b2fecf)

A single-page, offline-first interface for running multi-agent meetings locally with Ollama. Everything is contained in one HTML file—no build steps or servers required.

## Quick start
1. **Download the HTML.** Grab `OllamaMultiAgent v7.html` (or clone this repository) and keep the file on your machine.
2. **Open it in your browser.** Double-click the HTML file or drag it into a browser window. The entire UI runs locally.
3. **Install and run Ollama.** MultiAgent Meeting relies on your local Ollama runtime for inference. Install Ollama and keep the service running in the background while you use the app. The experience stays offline because every call targets your local runtime. [Download Ollama](https://ollama.com/download/windows).
4. **Allow browser access (CORS).** Set `OLLAMA_ORIGINS=*` (or a more restrictive value that includes `file://`) before starting Ollama so the standalone HTML can reach the API.

## Setting `OLLAMA_ORIGINS` on Windows
1. Open **Control Panel → System → Advanced system settings**.
2. Click **Environment Variables…**.
3. Under **User variables** (or **System variables** to apply globally), choose **New…**.
4. Add the following:
   - **Variable name:** `OLLAMA_ORIGINS`
   - **Variable value (for development):** `*` (you can tighten this to `http://localhost:8000` later)
5. Click **OK** to close all dialogs.

You're ready to run multi-agent meetings locally—no cloud APIs needed.
