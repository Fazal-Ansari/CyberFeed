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
## 💻 **Installation Instructions** ⚙️

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/cyber-attacks-analytics-dashboard.git
   cd cyber-attacks-analytics-dashboard
