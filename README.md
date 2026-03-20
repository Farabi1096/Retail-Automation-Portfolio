# Retail Automation Portfolio
**[Your Name] / portfolio** &nbsp; [![Back to Profile](https://img.shields.io/badge/←_Back_to_Profile-FF0000?style=flat-square&logoColor=white)](https://github.com/Farabi1096/portfolio) [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/farabi-hsn/)

---

### 🛠️ Expertise
![Automation](https://img.shields.io/badge/Automation-Apps_Script_%7C_VBA-FF0000?style=flat-square&logoColor=white) ![AI Integration](https://img.shields.io/badge/AI_Integration-Gemini_API_%7C_Vision-000000?style=flat-square&logoColor=white) ![Data Architecture](https://img.shields.io/badge/Architecture-Hierarchy_Logic-FF0000?style=flat-square&logoColor=white)

---

### ![Project](https://img.shields.io/badge/Project-Retail_Outlet_Display_AI_Audit-FF0000?style=for-the-badge&logo=googlecloud&logoColor=white)

> **Problem:** Retail audit teams struggle with thousands of unorganized outlet photos, making it impossible to verify if "Shelf Talkers" are present or if products are stocked correctly in real-time.  
> **Solution:** A complete end-to-end pipeline using a Web App and Gemini AI to automatically audit display modality, log SKU data, and organize files into a strict business hierarchy.

---

#### 🔄 Step-by-Step Implementation

**Step 1: Field Submission (Web App)** Sales officers use a custom-built web interface to capture and upload display photos. The app captures critical metadata like **Area, Town, and DB Code** automatically to ensure data integrity from the start.
<p align="center">
  <img src="images/Web_App.jpg" width="90%" alt="Web App Interface" />
</p>

**Step 2: AI Logic & Automation (Apps Script + Vision API)** The core engine uses **Google Apps Script** to send images to the **Gemini Vision API**. The AI identifies if the branding is compliant and calculates product availability. Simultaneously, a script renames the file using a clean hierarchy: `Area > Town > DB_Code > Timestamp`.
<p align="center">
  <img src="images/App_Script_API.jpg" width="90%" alt="Apps Script and AI Logic" />
</p>

**Step 3: Database & Monitoring (Google Sheets)** All AI findings—including compliance status and stock quantities—are instantly logged into a master Google Sheet. This structured data serves as the backend for management reports and KPI tracking.
<p align="center">
  <img src="images/Google_Sheet.jpg" width="90%" alt="Google Sheet Database" />
</p>

---

#### 🧠 Technical Highlights
* **Vision AI Audit:** Automatically detects "Shelf Talker" presence and filters out non-relevant or duplicate images.
* **Intelligent File Hierarchy:** Solves "cloud clutter" by organizing every upload into regional folders with standardized naming conventions.
* **Zero Manual Entry:** DB Names and Area details are pulled from the database based on the DB Code, reducing officer input time.

#### 💡 Business Impact
* **100% Audit Coverage:** Every single photo is checked by AI, eliminating the need for random spot checks.
* **Organized Assets:** Thousands of images are instantly searchable by Region or DB Code.
* **Data Accuracy:** Removed human bias from compliance reporting, ensuring 100% transparency in the field.

---
