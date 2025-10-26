<div align="center">
  <img src="images/logo_512.png" alt="Chat Outline for Gemini Logo" width="128"/>
  <br/>
  <a href="https://github.com/google-gemini/gemini-cli">
    <img src="https://img.shields.io/badge/Made%20with-Gemini%20Cli-4285F4?style=for-the-badge&logo=google-gemini&logoColor=white" alt="Made with Gemini-Cli"/>
  </a>
</div>

# Chat Outline - A Firefox Extension for Gemini

This is a simple Firefox extension that adds a clickable outline to your [Gemini](https://gemini.google.com) chat history, making it easier to navigate long conversations.

## Features

-   **Clickable Outline**: Generates a list of all your prompts in a conversation.
-   **Easy Navigation**: Click any prompt in the outline to instantly scroll to that point in the chat.
-   **Pin the Outline**: Keep the outline popover open and visible while you scroll and interact with the chat.
-   **Quick-Quote**: Quickly quote a specific part of a message to ask a follow-up question.
-   **Minimalist UI**: The outline is accessible via a simple icon and can be opened or closed.
-   **Light & Dark Theme**: Automatically adapts to the Gemini website's theme.
-   **Chat Tagging System**: Organize and manage your chats with custom tags.
-   **Interactive Tag Management**: Add, remove, and rename tags directly from the interface with intuitive buttons (green '+' to add, red '×' to remove, pencil '✏️' to rename).

## Install from Mozilla Add-ons

You can download and install the extension directly from [Mozilla Add-ons](https://addons.mozilla.org/).

## How to Install (from source)

1.  Clone or download this repository.
2.  Open Firefox and navigate to `about:debugging#/runtime/this-firefox`.
3.  Click **Load Temporary Add-on**.
4.  Select the `manifest.json` file in this directory.

The extension's icon will now appear in the toolbar of the Gemini chat window.

---

## AI-Assisted Development Workflow (Recommended)

To maintain consistency and development speed, we highly recommend using an AI programming assistant like **Gemini CLI**, GitHub Copilot, or others for your contributions.

The key to success is providing the AI with the right context. Our project's "source of truth" for its architecture is the technical documentation.

### Recommended Steps

1.  **Define Your Goal**: Have a clear idea of the feature or bug fix you want to implement.

2.  **Gather Context**: Your primary context files are:
    *   `docs/tech.md` (The project's architectural blueprint)
    *   The specific file(s) you intend to modify (e.g., `content.js`, `styles.css`).

3.  **Write a Clear Prompt**: Describe your goal in detail to the AI. For example:
    > "I want to add a 'copy to clipboard' button next to each item in the outline list inside `#gemini-toc-list`. When a user clicks this button, the text content of that specific prompt should be copied to their clipboard. Please ensure the new button's styling matches the existing UI and that all logic adheres to the patterns described in the provided technical documentation and existing code."

4.  **Execute and **Review****:
    *   Use your preferred AI tool to generate the code.
    *   **This is the most critical step.** Always manually review, test, and refine the AI's output. You are the author of the final code, and you are responsible for its quality and correctness.

### Example using Gemini CLI

If you wanted to implement the "copy button" feature described above, you could use a command like this:

```bash
gemini

@docs/tech.md {YOUR PROMPT}
```

This command tells Gemini to edit using your prompt, with the additional context of the technical documentation.
