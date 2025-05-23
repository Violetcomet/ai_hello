# Your Personal AI Cloud Companion

## Description
Bring a touch of magic to your digital space with this animated, cloud-themed AI chat widget! Engage in quick, concise conversations, get creative ideas, or receive uplifting messages, all displayed with a smooth, dynamic text animation. Perfect for Notion dashboards or personal websites.

## Features
✨ **Animated Text Display:** Smoothly transitions AI responses for an engaging visual experience.
☁️ **Cloud-Themed Design:** A gentle, aesthetic interface that's easy on the eyes.
💬 **Interactive Chat:** Ask questions and receive concise AI-generated responses.
💡 **Idea Generation:** Click a button to get creative ideas on any topic.
😊 **Mood Uplifter:** Get short, encouraging messages to brighten your day.
🚀 **Easy to Embed:** Designed to be seamlessly integrated into Notion pages, personal websites, and more.
📏 **Responsive Layout:** Adapts to different screen sizes for optimal viewing.

## How to Use & Embed in Notion (or other platforms)

This widget is a static HTML file that needs to be hosted online to be embedded. GitHub Pages is a great, free option!

### 1. Save Your Code
   * Create a new folder on your computer (e.g., `ai-cloud-widget`).
   * Save the HTML code (provided previously) into this folder as `index.html`. It's crucial to name it exactly `index.html`.

### 2. Host on GitHub Pages
   * **Create a GitHub Repository:**
     * Go to [github.com](https://github.com/) and log in.
     * Click the **"+"** icon in the top right and select **"New repository."**
     * Give it a name (e.g., `ai-cloud-widget`). Make it **Public**.
     * You can optionally check "Add a README file" now, or add this README later.
     * Click **"Create repository."**
   * **Upload Your `index.html`:**
     * On your new repository page, click **"Add file"** > **"Upload files."**
     * Drag and drop your `index.html` file (and the `README.md` if you created it) into the upload area.
     * Scroll down and click **"Commit changes."**
   * **Enable GitHub Pages:**
     * Go to the **"Settings"** tab of your repository.
     * Under "Build and deployment," choose **"Deploy from a branch."**
     * Under "Branch," select `main` (or `master` if your repository uses that) and choose the `/ (root)` folder.
     * Click **"Save."**
   * **Get Your Live URL:** After a moment, GitHub will deploy your site. You'll see a message like: "Your site is published at `https://yourusername.github.io/your-repo-name/`". This is the URL you will use to embed!

### 3. Embed in Notion
   * Open your Notion page.
   * Type `/embed` in an empty block and press `Enter`.
   * Paste the public URL you got from GitHub Pages into the prompt.
   * Click "Embed link."
   * You can resize the embedded widget in Notion by dragging its corners.

## Customization
You can easily customize aspects of the widget by editing the `index.html` file:

* **Your Name:**
    * Find `const userName = "Ishan";` in the `<script>` section.
    * Change `"Ishan"` to your desired name.
* **AI Responses:**
    * The prompts for `sendMessage`, `generateIdeas`, and `liftSpirits` in the JavaScript are designed to encourage concise responses. You can modify these prompts if you want longer or different types of AI output.
* **Styling:**
    * Adjust the CSS within the `<style>` tags to change colors, fonts, sizes, and animations.
* **Gemini API Key:**
    * The `apiKey` variable in the `callGeminiAPI` function is left empty (`const apiKey = "";`). When deployed via Google's platforms (like Canvas), this is automatically populated. If you're hosting this on a general web server and want to use your own Google Cloud API Key, you would insert it here. **However, exposing API keys directly in client-side code (like this) is generally not recommended for production applications.** For simple personal use, it might be acceptable, but be aware of the security implications.

## Technologies Used
* **HTML5:** Structure of the widget.
* **CSS3:** Styling and animations.
* **JavaScript (ES6+):** Interactivity and AI integration.
* **Tailwind CSS (CDN):** For utility-first styling.
* **Google Gemini API:** Powers the AI responses.

## License
This project is open-source and available under the [MIT License](LICENSE.md).

## Contact
If you have any questions or suggestions, feel free to reach out via [Your GitHub Profile Link] or [Your Email - Optional].