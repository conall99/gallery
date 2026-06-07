# Advanced Guide: Mastering Gemini CLI in Visual Studio Code

Welcome to your expert-level guide on maximizing the potential of the Gemini CLI within VS Code. Now that you have successfully connected the CLI to your workspace, this document will walk you through advanced workflows, context management, and best practices to supercharge your coding experience.

## 1. Understanding Workspace Context

The true power of the Gemini CLI lies in its contextual awareness. It doesn't just answer questions; it observes your coding environment.

* **Active Selection:** The CLI automatically reads whatever text you have highlighted in your active editor window (up to an impressive 16KB of text).
* **Recent Files Tracker:** It keeps track of the 10 files you have most recently opened or modified. This means you can ask questions about how different parts of your codebase interact without explicitly pasting the code.

**Expert Tip:** To verify exactly what context the CLI currently holds, use the `/ide status` command. This ensures the AI isn't hallucinating and is looking at the correct files before you issue a complex refactoring command.

## 2. Core Workflows and Commands

Instead of treating the CLI like a search engine, treat it like a pair programmer sitting next to you.

### Generating New Code
When writing new features, open a blank file or place your cursor where you want the new code to go. Be specific about your architectural requirements.

* **Example Prompt:** *"Generate a React functional component for a user login form. Use Tailwind CSS for styling, include state management for email and password using `useState`, and add basic client-side validation to ensure the email is properly formatted before submission."*

### Refactoring Existing Code
Highlight the block of code you want to improve. You don't need to copy it into the terminal. 

* **Example Prompt:** *"Refactor this highlighted JavaScript function to use async/await instead of Promises. Also, extract the error handling into a separate utility function to keep this block clean."*

### Debugging and Error Resolution
If you encounter a stack trace or an unexpected bug, highlight the problematic code or the error output itself.

* **Example Prompt:** *"I'm getting a 'NullReferenceException' on line 42 of this highlighted block. Can you explain why this might be happening given the current state variables, and propose a fix?"*

## 3. The Native Diffing Experience

When you ask the CLI to write or modify code, it utilizes VS Code's native diffing engine instead of just printing text in the terminal.

1. **Triggering the Diff:** Issue your prompt (e.g., *"Add inline documentation to this class"*).
2. **Reviewing Changes:** VS Code will open a split-screen Diff Editor. The left side shows your original code; the right side shows Gemini's proposed changes.
3. **Manual Tweaking:** You are not locked into accepting the whole block. You can manually type and edit within the right-hand (proposed) pane if you want to tweak Gemini's logic.
4. **Accepting Changes:** * Save the file (`Ctrl+S` or `Cmd+S`).
   * Click the 'Checkmark' or 'Accept' button in the editor title bar.
   * Type `yes` or `y` in the Gemini CLI terminal.

## 4. Pro Tips for Maximum Efficiency

* **Keep Selections Focused:** While the CLI can read up to 16KB, you will get much better, more accurate results if you highlight only the specific function or class you want to modify.
* **Iterative Prompting:** Don't ask for a monolithic script in one go. Build it step-by-step. *"First, build the database schema."* -> (Accept Diff) -> *"Now, write the CRUD operations for this schema."*
* **Set the Guidelines Early:** If your project has specific linting rules or naming conventions, tell the CLI early in your session. *"For this session, ensure all Python variables use snake_case and all functions include docstrings."*

Happy Coding!
