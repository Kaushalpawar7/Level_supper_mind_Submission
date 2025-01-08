
### **README.md**  

# **Social Media Performance Analytics with Langflow and Astra DB**  

This project provides a powerful and user-friendly solution to analyze social media engagement using **Langflow** for flow-based AI-driven insights and **DataStax Astra DB** for scalable, cloud-based data storage. It enables users to input post types (e.g., reels, carousels, static images) and topics to generate performance analytics and actionable insights for platforms like **Instagram and YouTube**.  

---

### **Project Features**  
- **Automated Engagement Metrics Calculation**:  
  Fetches engagement data from mock social media datasets and calculates average likes, comments, shares, and views for different post types.  
- **Cross-Platform Performance Insights**:  
  Compare Instagram and YouTube analytics to optimize content strategies.  
- **AI-Powered Insights**:  
  Leverages Google Generative AI (Gemini) for dynamic, data-driven content suggestions, best timing, and hashtag performance.  
- **Interactive Flow with Langflow**:  
  Input post type and topic directly through a Langflow interface to receive immediate insights.  

---

### **Getting Started**  

#### **1. Online Version Using Langflow**  
1. Visit the [Langflow website](https://www.langflow.org/) and log in or create an account.  
2. Upload the flow file from this repository:  
   - `Social Media Analytics Flow.json`.  
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
- Upload a social media dataset to Astra DB.  
- Use Langflow to input post types and topics.  
- The flow queries Astra DB for engagement metrics and uses AI to generate concise, percentage-based insights.  

**Example Output**  
- *"Reels on tech topics generate 2x more views than carousel posts. 📈"*  
- *"Top Instagram hashtags for coding: #CodeLife #TechTrends 🏷️"*  

---

### **Contact**  
For questions or feedback, please contact:  
- **Kaushal Pawar**  
- **Email**: [kaushalpawar2346@gmail.com](mailto:kaushalpawar2346@gmail.com)  
