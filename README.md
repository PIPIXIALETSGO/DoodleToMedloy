
# Doodle to Melody: Interactive Drawing Meets Music

**Author:** Jiahao Wu  
**GitHub Repository:** [https://github.com/PIPIXIALETSGO/Cart398](https://github.com/PIPIXIALETSGO/Cart398)

---

## 📜 Abstract

**Doodle to Melody** is an interactive project that connects creative sketching with music through machine learning and API integration. Users draw doodles on a p5.js-powered sketch board, which are classified in real time by the pre-trained **DoodleNet** model (trained on Google’s *Quick, Draw!* dataset).  

The top classification label is used as a keyword to query the **Spotify API**, which fetches and plays a related song while displaying detailed song and artist information. The interface includes playful elements like doodle-style visuals, an animated gramophone, a real-time label notebook, and a song calendar.  

This project explores **embodied digital creativity** by connecting user-generated art with personalized audio, highlighting the potential of cross-modal interaction systems that blend drawing and music into a unified creative experience.

---

## 🧭 1. Introduction

This project explores the intersection of **human-computer interaction (HCI)**, **creative AI**, and **digital art**. By transforming freehand sketches into music, it bridges visual creativity with auditory exploration in an intuitive and engaging way.

Leveraging the pre-trained **DoodleNet** sketch recognition model, the system classifies drawings and retrieves music using Spotify’s API. Unlike similar projects that focus on either generative music (e.g., Google Magenta) or simple sketch-to-sound mappings (e.g., DrawSound), this project uniquely connects **real-time sketch classification** with **dynamic music retrieval**.  

The goal is to inspire creativity by offering an interactive platform that blurs the boundaries between visual art and music — showcasing how AI and creative coding can create **hybrid, user-driven media experiences**.

---

## 🎨 2. Project Description

Users draw doodles on a **web-based sketch board**. The system processes the drawing through a CNN-based ML model and returns the top three classification labels. The highest-confidence label is then used to search for and play a song via the **Spotify API**.  

This real-time pipeline enables a direct, embodied interaction between **visual expression** and **musical feedback**.

### 🛠️ Technologies Used

- **p5.js** – Drawing interface for sketch creation and interaction.  
- **TensorFlow.js** – Client-side deployment of the DoodleNet CNN model.  
- **Spotify Web API** – Fetches and plays music related to the classified doodle.  
- **HTML/CSS** – Interface structure and visual design.

**Hardware:**  
Only a standard computer, mouse, and web browser are required — making the system accessible to anyone.

---

## 🤖 Machine Learning Implementation

### 🔍 ML Task: Classification  
The project uses a **Convolutional Neural Network (CNN)** to classify sketches into one of 345 categories. It returns the top three labels ranked by confidence.

### 📊 Model: DoodleNet  
DoodleNet, trained on Google’s *Quick, Draw!* dataset, is highly optimized for sketch recognition. It processes input images through multiple convolution and pooling layers to identify features and predict labels.

### 🧠 Infrastructure  
The model runs **entirely in the browser** via TensorFlow.js — no external servers required.

---

## 📚 Training Data

- **Dataset:** [Quick, Draw!](https://quickdraw.withgoogle.com/data)  
- **Categories:** 345+ objects and concepts (e.g., “cat,” “tree,” “airplane”)  
- **Examples:** Thousands of sketches per category, ensuring diverse recognition capabilities.

---

## 🔌 System Integration

The system integrates multiple components into a seamless experience:

1. **Sketching Interface** – p5.js canvas for drawing input.  
2. **ML Model** – DoodleNet classifies the sketch and returns labels.  
3. **Spotify API** – Uses top label as a keyword to play a related song.  
4. **UI Feedback** – Displays classification results and song details.

---

## 🧱 Development Stages

- **Initial Proposal:** Explore Magenta for custom model training with Unreal Engine output.  
- **Early Development:** Attempted Python-based model training.  
- **Pivot:** Switched to TensorFlow.js and pre-trained DoodleNet to accelerate progress.  
- **Final Implementation:** Consolidated all functionality into a single web application for simplicity and reliability.

---

## ⚙️ Challenges & Solutions

- **Python Complexity:** Switched to JavaScript for faster development.  
- **Time Constraints:** Used pre-trained models to save training time.  
- **Cross-Platform Issues:** Focused on a single web app to avoid integration complexity.

---

## ✅ Successes

- **Rapid Development:** Leveraged existing tools and libraries for quick progress.  
- **Seamless Experience:** Unified system with sketch recognition and music playback.  
- **Accessible & Engaging:** Intuitive interaction that blends art and sound.

---

## 📚 Key Learning Experiences

- **Adaptability:** Switching technologies accelerated development.  
- **System Design:** Consolidating functionality improved reliability.  
- **Resource Utilization:** Leveraging pre-trained models enhanced innovation.

---

## 🚀 Future Improvements

### 🧠 Enhanced ML Capabilities
- Train custom CNNs for better accuracy and broader categories.  
- Implement multi-label classification.  
- Add camera-based sketch recognition.

### 🎶 Expanded Music Features
- Feedback-driven song selection.  
- Mood-based matching and playlist generation.  
- Support for additional music platforms (e.g., Apple Music, YouTube Music).

### 🎨 Visual & UI Enhancements
- Dynamic animations linked to recognized sketches.  
- Predictive sketch completion.  
- Community-driven drawing comparisons.

### 🖐️ Advanced Interaction Modalities
- Voice or gesture-based input.  
- Mobile/touchscreen support.

### 👥 Collaborative Features
- Real-time shared sketchboards.  
- Community playlists and sketch challenges.

### 🌐 Cross-Media Integrations
- Sketch-to-art generation.  
- Dance or movement visualizations.  
- Storytelling based on sketches.

---

## 📁 Project Structure

```
Cart398/
├── index.html          # Main web application
├── sketch.js           # p5.js drawing logic
├── model.js            # TensorFlow.js model integration
├── spotify.js          # Spotify API integration
├── styles.css          # UI styling
└── assets/             # Visual and UI elements (images, icons, etc.)
```

---

## 📦 Installation & Usage

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/PIPIXIALETSGO/Cart398.git
   cd Cart398
   ```

2. **Open `index.html`** in a modern browser.

3. **Start Drawing:**  
   - Draw a doodle with your mouse.  
   - Watch the model classify your sketch.  
   - Enjoy a related song from Spotify.

---

## 🎉 Conclusion

**Doodle to Melody** demonstrates how **machine learning, creative coding, and APIs** can come together to create a playful, expressive, and deeply interactive experience. It is a testament to the power of cross-modal systems — where art and technology merge to inspire new forms of creativity.
