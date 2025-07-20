# 🌍 Travel Planner App

## 📖 About This Project
The **Travel Planner App** helps users plan their trips by providing:
- **Weather forecasts** for their destination 📊
- **Beautiful images** of their destination 🖼️
- **A countdown** to the trip ⏳
- **Offline support** with Service Workers 🚀

This project is built using **JavaScript (ES6+), Webpack, Node.js, Express, and Bootstrap**.

---

## ✅ Features
✔️ Enter your **destination** and **departure date**  
✔️ Fetch the **latest weather forecast**  
✔️ Get a **random image of the destination**  
✔️ **Works offline** with Service Workers  
✔️ **Live updates** using Webpack Dev Server  
✔️ **Responsive UI** with Bootstrap  

---

## 🛠 Prerequisites
To run this project, make sure you have installed:
- **Node.js v18+** (Check with `node -v`)
- **NPM v8+** (Check with `npm -v`)

---

## 🚀 Technologies Used
| **Technology**   | **Purpose** |
|-----------------|------------|
| **JavaScript (ES6+)** | Frontend logic |
| **Node.js & Express** | Backend API |
| **Webpack** | Module bundler |
| **SCSS** | Styles |
| **Bootstrap** | Frontend styling & responsiveness |
| **jQuery** | DOM manipulation & Bootstrap integration |
| **Workbox** | Service Worker for offline support |
| **Jest** | Unit testing |
| **Geonames API** | Fetch city coordinates |
| **Weatherbit API** | Fetch weather forecast |
| **Pixabay API** | Fetch destination images |

---

## 🎨 UI & Styling (Bootstrap)
This project uses **Bootstrap v5.3.3** to ensure a **responsive and modern design**.  
### **Why Bootstrap?**
✔️ Provides **pre-built UI components**  
✔️ Enables **mobile-first design**  
✔️ Simplifies styling with **grid system & utility classes**  
✔️ Includes **modals, buttons, and form styles**  

**Imported Bootstrap in `index.js`:**
```js
import 'bootstrap/dist/css/bootstrap.css';
import 'bootstrap';
📌 Bootstrap is installed via NPM:

npm install bootstrap

📌 Official Documentation:
🔗 https://getbootstrap.com/

📥 Installation & Setup
1️⃣ Clone the Repository
Open your terminal and run:

sh
Copy
git clone https://github.com/yourusername/travel-planner-app.git
cd travel-planner-app
2️⃣ Install Dependencies
Run:

sh
Copy
npm install
3️⃣ Set Up API Keys
Create a .env file in the project root.
Add the following API keys (Replace with your actual keys):
sh
Copy
GEONAMES_USER=your_geonames_username
WEATHERBIT_KEY=your_weatherbit_api_key
PIXABAY_KEY=your_pixabay_api_key
🏗 Running the Project
💻 Development Mode (Hot Reload)
To start the app in development mode with live reloading, run:

sh
Copy
npm run dev
Then open:
🔗 http://localhost:8081/

🚀 Production Mode
Build the project:
sh
Copy
npm run build
Start the Express server:
sh
Copy
npm start
Open the app at:
🔗 http://localhost:8080/
🧪 Running Tests
To test the app using Jest, run:

npm test
🛠️ Troubleshooting
1️⃣ Error: Module not found: Can't resolve 'main.scss'
✅ Fix: Ensure main.scss is inside src/client/styles/ and imported correctly in index.js:

js
Copy
import './styles/main.scss';
2️⃣ Error: GenerateSW has been called multiple times
✅ Fix: Ensure GenerateSW is only included in webpack.prod.js and not in webpack.config.js.

3️⃣ Error: Module parse failed: Unexpected character '@' (Bootstrap)
✅ Fix: Ensure Webpack is configured to handle CSS files by adding this rule in webpack.config.js:

js
Copy
module: {
    rules: [
        { test: /\.css$/, use: ['style-loader', 'css-loader'] }
    ]
}
📜 License
This project is open-source and available under the MIT License.
👤 Developed by Diana Naseer.

