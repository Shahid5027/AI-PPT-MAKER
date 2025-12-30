# 🤖 AI Presenter: Gesture-Controlled Presentation Generator

A futuristic, single-file web application that generates full slide decks using AI, controllable via webcam hand gestures ("Minority Report" style).

![Image](https://github.com/user-attachments/assets/5e2da767-6382-43ed-9a73-be0e4cffdd11)

## ✨ Features

### 🧠 **Smart AI Generation**
- **Topic-to-Slides:** Simply type a topic (e.g., *"Future of Mars"*).
- **Smart Slide Count:** Automatically detects requested length from your prompt (e.g., *"History of Rome **8 slides**"*).
- **Dual AI Engine:** - **Google Gemini 1.5 Flash:** Generates structured slide content (Titles, Bullet points).
  - **Pollinations.AI (Flux Model):** Generates high-quality, artistic visuals for every slide.

### ✋ **Gesture Control**
- **Touch-Free Navigation:** Use your webcam to control slides.
  - **Next Slide:** Raise your **Right Hand** ✋.
  - **Previous Slide:** Raise your **Left Hand** 🤚.
- **Privacy First:** Includes a toggle to disable the camera/detection loop when not presenting.

### ✏️ **Full Editor Mode**
- **Live Editing:** Click any text on any slide to edit it instantly.
- **Custom Images:** Don't like the AI image? Click **"📷 Change Image"** to upload your own picture.
- **State Persistence:** Edits are saved automatically as you navigate.

### 🎨 **Themes & Export**
- **3 Visual Themes:** Retro (Cyberpunk), Educational (Clean), and Fun (Creative).
- **PowerPoint Export:** Download your deck as a `.pptx` file with all images and text preserved.
- **PDF Viewer:** Upload and present existing PDF files using gesture controls.

---

## 🚀 Getting Started

This project is built as a **Single File Application**. No Node.js backend, Python server, or build step is required.

### Prerequisites
* A modern web browser (Chrome, Edge, Firefox).
* An internet connection (for AI generation).

### Installation
1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/yourusername/ai-presenter.git](https://github.com/yourusername/ai-presenter.git)
    ```
2.  **Open the file:**
    Double-click `index.html` to open it in your browser.

### 🔑 Configuration (API Keys)
To make the AI generation work, you must add your own API keys in the `index.html` file (Script section):

1.  Open `index.html` in a code editor.
2.  Find the `// --- CONFIG ---` section (approx line 350).
3.  Insert your keys:
    ```javascript
    const apiKey = "YOUR_GEMINI_API_KEY"; 
    const POLLINATIONS_KEY = "YOUR_POLLINATIONS_KEY"; // Optional, usually free
    ```
    * *Get a Gemini Key:* [Google AI Studio](https://aistudio.google.com/)
    * *Get a Pollinations Key:* [Pollinations.AI](https://pollinations.ai/)

---

## 🎮 How to Use

1.  **Generate Slides:**
    * Type a topic in the input box.
    * *(Optional)* Specify slide count: "The Beatles **10 slides**".
    * Click **"Generate Presentation"**.
2.  **Presenting:**
    * Click the **"Gestures: OFF"** button to enable the webcam.
    * Stand back slightly so your upper body is visible.
    * Raise one hand clearly to switch slides (wait for the green border flash).
3.  **Editing:**
    * Click directly on the slide text to change it.
    * Hover over the image and click the button to upload a replacement.
4.  **Download:**
    * Click **"Download .pptx"** to save your work.

---

## 🛠️ Tech Stack

* **HTML5 / JavaScript (ES6 Modules)** - Core logic.
* **Tailwind CSS** - Styling and responsive design.
* **TensorFlow.js & MoveNet** - Real-time pose detection for gestures.
* **Google Gemini API** - Natural Language Processing.
* **PptxGenJS** - PowerPoint generation.
* **PDF.js** - PDF rendering.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

*Created with ❤️ by Shahid Ahmed Shariff*
