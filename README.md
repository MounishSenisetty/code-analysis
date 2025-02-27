# AI Code Analyzer for VS Code

This VS Code extension analyzes code for security vulnerabilities, coding issues, and best practices using **Google Gemini AI**. It highlights problems in the editor, provides explanations, and suggests fixes.

## Features
- ✅ **Static Code Analysis**: Identifies security flaws, redundant code, and poor coding practices.
- 🔍 **AI-Powered Analysis**: Uses **Google Gemini AI** to analyze code.
- 🚀 **Quick Fix Suggestions**: AI-generated fixes can be applied directly in VS Code.
- 💡 **Hover Explanations**: See detailed issue descriptions and fixes when hovering over problems.

## Installation
1. Clone this repository:
   ```sh
   git clone https://github.com/your-repo/ai-code-analyzer-vscode.git
   ```
2. Navigate to the extension folder:
   ```sh
   cd code-analysis
   ```
3. Install dependencies:
   ```sh
   npm install
   ```
4. Open VS Code and press `F5` to run the extension.

## Configuration
1. Open the `extension.js` file.
2. Replace `YOUR_GEMINI_API_KEY` with your actual **Google Gemini API key**:
   ```js
   const API_KEY = 'YOUR_GEMINI_API_KEY';
   ```
3. Save the file and restart VS Code.

## Usage
- Open any source code file in VS Code.
- Run the command **"Analyze Code"** from the Command Palette (`Ctrl+Shift+P`).
- Issues will be highlighted in the editor with AI-generated fixes.
- Hover over an issue to see explanations and suggestions.
- Click on an issue and apply the **Quick Fix** to resolve it.

## Example Output
**Before Analysis:**
```js
const userInput = req.query.user; // Potential SQL Injection Vulnerability
```

**After AI Suggestion:**
```js
const userInput = encodeURIComponent(req.query.user); // Secure against SQL Injection
```

## Troubleshooting
- Ensure you have a valid **Google Gemini API key**.
- Restart VS Code if the extension does not load correctly.
- Check the VS Code **Output Panel** for logs.


## Contributions
Contributions are welcome! Feel free to submit a PR or open an issue.

