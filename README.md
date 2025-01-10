### **README.md**

# **Social Media Performance Analytics with Langflow and Astra DB**

This project provides a comprehensive and user-friendly solution to analyze social media engagement using **Langflow** for flow-based AI-driven insights and **DataStax Astra DB** for scalable, cloud-based data storage. It enables users to input post types (e.g., reels, carousels, static images) and topics to generate performance analytics and actionable insights for platforms like **Instagram and YouTube** using an advanced agentic architecture.

---

### **Project Features**

- **Automated Engagement Metrics Calculation**:  
  Fetches engagement data from Instagram and YouTube datasets and calculates average likes, comments, shares, and views for different post types.

- **Cross-Platform Performance Insights**:  
  Compare analytics for Instagram and YouTube to optimize content strategies and identify the best-performing content.

- **AI-Powered Insights Using Agentic Structure**:  
  Utilizes three specialized AI agents:  
  1. **Data Retrieval Agent**: Queries Astra DB for relevant engagement metrics.  
  2. **Analytics Agent**: Computes performance metrics and cross-platform comparisons.  
  3. **Content Optimization Agent**: Leverages Google Generative AI (Gemini) for actionable suggestions, including ideal posting times, effective hashtags, and dynamic content ideas.

- **Interactive Flow with Langflow**:  
  Input post type and topic directly through a Langflow interface to receive immediate insights and AI-generated suggestions.

---

### **Getting Started**

#### **1. Online Version Using Langflow**
1. Visit the [Langflow website](https://www.langflow.org/) and log in or create an account.  
2. Upload the flow file from this repository:  
   - `Social Media Analyst.json`.  
3. Create a **vector database** in **Astra DB** and set up a **collection named "engagement"**.  
4. Generate an **Application Token** under the Astra DB Overview tab and replace the **AstraDB token** in the Langflow component with your credentials.  
5. Replace the **Gemini API key** in the Google Generative AI Model and Embedding components.

#### **2. Local Setup**
1. Create a virtual environment:  
   ```bash
   python -m venv .venv
   .\.venv\Scripts\activate
   ```
2. Install Langflow:  
   ```bash
   python -m pip install langflow
   ```
3. Run Langflow locally:  
   ```bash
   python -m langflow run
   ```
4. Access Langflow at [http://127.0.0.1:7860](http://127.0.0.1:7860) in your browser and follow the online setup steps.

---

### **How It Works**
- Upload a social media dataset for both Instagram and YouTube to Astra DB.
- Use Langflow to input post types and topics.
- The flow uses a three-agent structure to:
  1. **Retrieve data**: Queries Astra DB for engagement metrics.
  2. **Analyze data**: Computes detailed engagement statistics.
  3. **Optimize content**: Generates dynamic content suggestions and key performance indicators.

**Example Output**
- *"Reels on tech topics generate 2x more views than carousel posts on Instagram. 📈"*
- *"YouTube videos on technology trends have 40% higher average watch time compared to general topics. 📺"*
- *"Top Instagram hashtags for coding: #CodeLife #TechTrends 🟧"*

---

### **Contact**
For questions or feedback, please contact:
- **Kaushal Pawar**
- **Email**: [kaushalpawar2346@gmail.com](mailto:kaushalpawar2346@gmail.com)

