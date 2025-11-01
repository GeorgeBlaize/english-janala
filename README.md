# English is Easy! — Interactive Vocabulary Learning Platform  

**English is Easy!** is an interactive, web-based English learning platform designed to help beginners improve their vocabulary through structured lessons, dynamic content, and engaging visuals.  
Built with **HTML5**, **CSS3**, **JavaScript (ES6)**, and powered by the **Programming Hero OpenAPI**, this project promotes learning English in a fun and interactive way — starting from Level A and beyond.  

---

## 🌐 Live Demo  
👉 [https://georgeblaize.github.io/english-janala/]

---

## 🧩 Features  

### 🏠 **Home / Banner Section**
- Beautiful hero banner with Bengali description text.  
- Login form for personalized access (Demo Password: `123456`).  
- Clean, minimal layout promoting ease of use.  

### 🧭 **Navigation Bar**
- Fixed, responsive navbar that appears after login.  
- Buttons for: **FAQ**, **Learn**, and **Logout**.  
- Smooth scrolling between sections.  

### 📘 **Vocabulary Learning**
- Fetches lessons dynamically from the **Programming Hero Vocabulary API**.  
- Displays words with pronunciation, meaning, example, and synonyms.  
- Includes sound icons (🔊) for pronunciation via **SpeechSynthesis API**.  
- View full details in a modal popup with “Complete Learning” confirmation.  

### 💡 **Interactive Lessons**
- Lesson buttons are generated dynamically using API calls.  
- Users can select different levels to view vocabulary lists.  
- Active lesson highlighting and loading indicators.  

### ❓ **FAQ Section**
- Common questions about learning English and platform usage.  
- Provides helpful insights for new users.  

### 🔒 **Login & Logout System**
- Simple client-side authentication for demonstration purposes.  
- Login success unlocks learning sections and navbar.  
- Logout confirmation using **SweetAlert2** popups.  

### 🎨 **Responsive UI**
- Clean, modern design with Bengali font support (`Noto Sans Bengali`).  
- Fully responsive across desktop, tablet, and mobile devices.  

### 📞 **Footer**
- Includes brand identity in English & Bengali.  
- Social media icons with links (Facebook, YouTube, Instagram, GitHub).  
- “Follow Us” section for user engagement.  

---

## 🛠️ **Technologies Used**

| Category | Tools / Libraries |
|-----------|------------------|
| **Frontend** | HTML5, CSS3, JavaScript (ES6) |
| **API Integration** | [Programming Hero Vocabulary API](https://openapi.programming-hero.com) |
| **UI Enhancements** | SweetAlert2 |
| **Speech Engine** | Web Speech API (`speechSynthesis`) |
| **Fonts** | Noto Sans Bengali (Google Fonts) |
| **Icons & Assets** | Local PNG assets (`assets/` folder) |

---

## 🧠 **How It Works**

1. 🏁 **Login** using your name and password (`123456`).  
2. 🧭 The navigation bar and lessons become visible after successful login.  
3. 📚 Choose a **Lesson** — words and details are fetched from the API dynamically.  
4. 🔊 Click the sound icon to hear pronunciation using **SpeechSynthesis**.  
5. ℹ️ Click the info icon to view detailed meaning, synonyms, and examples.  
6. ✅ Click “Complete Learning” to close the modal and continue.  
7. 🚪 Click “Logout” to exit safely (SweetAlert2 confirmation included).  

---

## 📂 **Project Structure**

english-is-easy/
│
├── index.html # Main project file
├── assets/ # Image and icon assets
│ ├── logo.png
│ ├── hero-student.png
│ ├── fb-thumb.png
│ ├── youtube-thumb.png
│ ├── instagram-thumb.png
│ ├── github-thumb.png
│ ├── fa-book-open.png
│ ├── fa-circle-question.png
│ ├── fa-arrow-right-from-bracket.png
│
└── README.md # Project documentation

yaml
Copy code

---

## 🧾 **APIs Used**

### 1. Get All Levels  
GET https://openapi.programming-hero.com/api/levels/all

pgsql
Copy code

### 2. Get Words by Level  
GET https://openapi.programming-hero.com/api/level/{level_no}

shell
Copy code

### 3. Get Word Details by ID  
GET https://openapi.programming-hero.com/api/word/{id}

yaml
Copy code

---

## ⚙️ **Setup Instructions**

1. **Clone this repository**
   ```bash
   git clone https://github.com/your-username/english-is-easy.git
Open the project folder

bash
Copy code
cd english-is-easy
Run the project

Simply open index.html in any modern browser.

Or use a local server for better experience:

bash
Copy code
npx live-server
🎬 Demo Login Credentials
Field	Value
Password	123456
Name	Any name you like

🧰 Dependencies
SweetAlert2 — For alerts and confirmations

Web Speech API — For pronunciation

Programming Hero OpenAPI — For vocabulary data

📱 Responsive Design
Uses flexbox and grid for layout.

Adapts gracefully to mobile, tablet, and desktop screens.

Adjusts footer and navbar layout responsively.

👨‍💻 Developer
Jonathan George Blaize Purification


💖 Acknowledgements
Programming Hero API Team for providing the free English vocabulary API.

SweetAlert2 for beautiful alert dialogs.

Google Fonts for Bengali text support.
