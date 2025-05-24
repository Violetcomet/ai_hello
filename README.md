# ☁️ Interactive AI Chat Widget for Notion ☁️

A customizable and animated chat widget designed to be embedded seamlessly into Notion, providing an interactive AI experience with a serene cloud theme. This widget is powered by the Google Gemini API, offering quick, context-aware responses and useful utilities.

## ✨ Features

* **Animated Text Display:** Smooth, typewriter-like animation for AI responses.
* **AI-Powered Responses:** Integrates with Google's Gemini API for dynamic, helpful chat.
* **Quick Action Buttons:**
    * **"Generate Ideas ✨":** Get creative ideas based on a topic you provide.
    * **"Lift My Spirits ✨":** Receive an encouraging message based on your mood.
* **User Chat Input:** Directly type and send messages to the AI.
* **Full Chat History:** Tracks the conversation within the current session.
* **Toggle Night/Day Mode 🌙☀️:** Switch between light and dark themes, with your preference saved locally in the browser.
* **New Chat 🔄:** Clear the current conversation and start fresh.
* **Delete History 🗑️:** Permanently delete all chat history with a confirmation step.
* **Copy History 📋:** Copy the entire conversation to your clipboard for easy sharing or saving.
* **Responsive Design:** Adapts fluidly to different screen sizes, from mobile to desktop.
* **Cloud-Themed UI:** A visually appealing interface with a calming cloud aesthetic, designed to complement your Notion workspace.

## 🚀 How to Use in Notion (Setup Guide)

To embed this interactive AI chat widget into your Notion page, follow these steps:

1.  **Host Your `index.html` File:**
    * The easiest way is to host your `index.html` file (containing this code) on **GitHub Pages**.
    * Create a GitHub repository, upload your `index.html` and your `Bầu trời.jpeg` image.
    * Go to your repository settings on GitHub, navigate to "Pages," and set your source to "main" (or your preferred branch) and select the `/ (root)` folder.
    * GitHub Pages will then provide you with a public URL (e.g., `https://yourusername.github.io/your-repo-name/`). Make sure your `Bầu trời.jpeg` image is also publicly accessible at its corresponding URL within your GitHub Pages site.

2.  **Copy the Public URL:**
    * Once your page is hosted (e.g., on GitHub Pages), copy the full public URL (e.g., `https://yourusername.github.io/your-repo-name/`).

3.  **Embed in Notion:**
    * Open your Notion page.
    * Type `/embed` and select the "Embed" block.
    * Paste the public URL you copied in the previous step into the embed block.
    * Click "Embed link."

4.  **Adjust Size:**
    * The widget will appear in your Notion page. You can drag the corners of the embed block to resize it to your preferred width and height, ensuring the chat area is maximized for your view.

## ⚙️ Customization

You can easily personalize several aspects of the widget by editing the `index.html` file:

1.  **Your Name:**
    * Change `const userName = "Ishan";` to your desired name (e.g., `"Alice"` or `"Master of Clouds"`). This name is used in the AI's greetings.

2.  **Background Image (`Bầu trời.jpeg`):**
    * Locate the `background-image` property in the `<style>` section.
    * Find the `url('https://placehold.co/800x600/D0EEF6/E0F2F7?text=Cloudy+Sky+Background')` part.
    * **Replace this placeholder URL with the direct public URL to your wallpaper image.** If you're using GitHub Pages, it might look something like `url('https://yourusername.github.io/your-repo-name/Bầu%20trời.jpeg')` (note: spaces in filenames might be replaced with `%20`).

3.  **Initial Greeting:**
    * Modify the second object in the `chatHistory` array (the one with `role: "model"`) to change the AI's initial greeting.
    * `{ role: "model", parts: [{ text: \`Hello, Master ${userName}! How can I assist you today?\` }] }`

4.  **AI Prompts & Logic:**
    * For advanced customization, you can modify the `callGeminiAPI` function and the prompts used in `generateIdeas`, `liftSpirits`, and `sendMessage` functions to alter the AI's behavior and response style.

## 🛠️ Technologies Used

* **HTML5:** For the basic structure of the widget.
* **CSS3:** For styling, animations, and responsive design.
* **JavaScript (ES6+):** For interactive elements, API calls, and animations.
* **Google Gemini API:** Powers the AI chat functionality.
* **Tailwind CSS:** Used for utility-first CSS classes (though mostly custom CSS is used here).

## 📄 License

This project is open-source. You can choose to add a specific license (e.g., MIT, Apache 2.0) to your repository. If no license is specified, standard copyright laws apply.

---

Feel free to contribute, open issues, or suggest further enhancements!