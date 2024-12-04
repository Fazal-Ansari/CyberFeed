# CyberFeed
# 🔐 **Cyber Attacks Analytics Dashboard** 

Welcome to the **Cyber Attacks Analytics Dashboard**! 🌐🔍 This project aggregates and analyzes the latest cybersecurity news related to cyber attacks, fraud, and incidents, displaying it in an interactive **dashboard** with visualizations. It uses **Python**, **Flask**, **Dash**, and **Plotly** to provide a user-friendly interface that makes cybersecurity data easier to explore and understand. 📊✨

The project consists of two main parts:
1. **Flask App**: Scrapes the latest news from cybersecurity-related websites and provides detailed summaries of the articles.
2. **Dash App**: Displays interactive charts and tables of the aggregated news data, allowing users to explore fraud categories and trends. 📈💡

---

## 🔍 **Project Features**

- 🌐 **Cybersecurity News Scraping**:
  - Scrapes articles from **cybersecurity-related websites** like **Krebs on Security**, **Cyberscoop**, and **The Hacker News**.
  - Extracts key information such as **title**, **date**, and **description** of the latest cyber incidents.
  - **Summarizes articles** using **Groq AI** to provide concise and useful overviews of each article. 🤖📝

- 📊 **Fraud Category Analytics**:
  - Aggregates tagged articles into categories like **Phishing**, **Malware**, **Social Engineering**, and more.
  - Generates **interactive charts** (Bar and Pie charts) to visualize the **fraud type distribution** using **Plotly**. 🔄📊

- 💾 **Downloadable Reports**:
  - Users can **download CSV reports** containing the scraped articles with their tags, summaries, and more.
  - **Download chart images** for offline use, so you can take your **fraud analytics** anywhere. 📥
---
## 🚀 **How It Works**

### **Step 1: Web Scraping** 📥
1. **Flask Scraping Functions**:
   - **Scrapes articles** from a list of cybersecurity-related websites using **BeautifulSoup**.
   - Extracts key information: **article title**, **publication date**, and **article description**.
   - **Tags articles** using pre-defined **fraud keywords** (e.g., **Phishing**, **Malware**, etc.) to categorize them based on detected threats.
2. **Groq AI Integration** 🧠:
   - Each article’s description is sent to **Groq AI** for **summarization**, making it easier to understand the key points.
   - The summarized text is presented to the user, providing a brief overview without reading the entire article. 📚💬
---
### **Step 2: Tagging Articles** 🏷️
1. **Keyword-Based Tagging**:
   - Articles are tagged based on matching keywords in their content (e.g., “crypto fraud”, “ransomware”).
   - Uses **regular expressions** to check for exact matches of predefined **fraud keywords**.
2. **Categories Assigned**:
   - Tags are dynamically assigned to each article, classifying them into categories like **Phishing**, **DDoS Attacks**, and more. 🔒
---
### **Step 3: Dash Dashboard** 📊
1. **Dashboard Layout**:
   - Displays an **interactive Bar chart** or **Pie chart** showing the distribution of fraud types.
   - Provides a **data table** with scraped articles, including **tags**, **description**, and **publication date**.

2. **User Interactivity**:
   - Users can switch between **Bar** and **Pie charts** to visualize the fraud distribution.
   - **Expandable descriptions** allow users to view or hide article summaries for detailed information. 🔄🔎
---
### **Step 4: Downloading Reports** 💾
- **CSV Report**: Users can **download a CSV** containing all tagged articles with their associated **fraud categories**.
- **Chart Image**: Users can download the current **chart image** (in PNG format) for offline analysis or record-keeping. 📥💼
---
## 🧑‍💻 **Technologies Used** 🛠️
- **Python** 🐍 (Flask, Dash, Requests, BeautifulSoup)
- **Plotly** 📊 (for interactive graphs)
- **Groq AI** 🤖 (for text summarization)
- **HTML & CSS** 🎨 (for styling the web interface)
---
📝 **Cyber Attacks Analytics Dashboard - Workflow** 🔄

  1️⃣ **Scraping News Websites** 🌐
      ↳ Websites scraped for latest articles:
          - Krebs on Security 🕵️‍♂️
          - Cyberscoop 💻
          - The Hacker News 📰

      ➡️ Extract article information:
          - Title 📝
          - Date 📅
          - Description 🧐
    
  2️⃣ **Summarizing Articles** 🤖
      ↳ Each article's description is summarized using **Groq AI**:
          - Short, concise overview 📚
    
  3️⃣ **Tagging Articles** 🏷️
      ↳ Articles are tagged based on fraud categories using predefined keywords:
          - Phishing 🐟
          - Malware 🦠
          - Social Engineering 🤔
          - More categories... 🔐

  4️⃣ **Storing and Organizing Data** 💾
      ↳ Articles and their tags are stored in a **DataFrame**:
          - Each article has its associated **tags**, **summaries**, and **dates**.
    
  5️⃣ **Data Visualization** 📊
      ↳ Data displayed using **Dash**:
          - Bar Chart 📊
          - Pie Chart 🍰
    
      ➡️ Charts display the distribution of fraud types:
          - Fraud categories on the x-axis (e.g., Phishing, Malware)
          - Counts of articles on the y-axis 📈
    
  6️⃣ **User Interaction** 🔄
      ↳ Users can:
          - Toggle between Bar/Pie charts 🔀
          - Expand/Collapse article summaries 🔍
    
  7️⃣ **Downloading Reports** 💾
      ↳ Users can download:
          - **CSV Report** 📥: Contains tagged articles and fraud categories
          - **Chart Image** 📸: PNG of the current chart
  
  8️⃣ **Final Output** 🎉
      ↳ Interactive dashboard with fraud insights and analytics. 📊🔒
-----------------------------------------------------
✨ **End Workflow** ✨

## 💻 **Installation Instructions** ⚙️

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/cyber-attacks-analytics-dashboard.git
   cd cyber-attacks-analytics-dashboard

📁 cyber-attacks-analytics-dashboard/
├── 📂 static/                # Static assets (CSS, images, etc.)
│   ├── 📄 background.gif     # Background GIF
│   └── 📄 styles.css         # Custom styles
├── 📂 templates/             # HTML templates
│   └── 📄 index.html         # Main template to display news
├── 📄 app.py                 # Flask app to run the backend
├── 📄 requirements.txt       # List of dependencies
└── 📄 README.md              # Project documentation


🎯 To-Do / Future Enhancements 🚀
 🌍 Add support for more news sources and fraud categories.
 📅 Implement a more advanced date handling system to better sort articles by date.
 🌐 Create a real-time scraper that automatically fetches and updates the news data.
 💬 Build a user feedback system to improve article summarization and tagging accuracy.

